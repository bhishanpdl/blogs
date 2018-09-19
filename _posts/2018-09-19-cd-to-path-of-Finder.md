---
layout: post
title: cd to the path of frontmost path in Finder
---

Date: Sep 19, 2018

Many times we need to open the Finder paths in the terminal. We can do in muliple ways: 

> open the terminal and type the whole path.


> If we have right click new terminal service: Right click and open in new terminal.

However, today I found a new way to open current finder path in terminal using bash function inside our
bashrc file.

The required function is presented below:
```bash
cdf() {
      target=`osascript -e 'tell application "Finder" to if (count of Finder windows) > 0 then get POSIX path of (target of front Finder window as text)'`
        if [ "$target" != "" ]; then
            cd "$target"; pwd
        else
            echo 'No Finder window found' >&2
        fi
}
```
