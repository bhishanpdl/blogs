---
layout: post
title:  Use TODO list in Markdown
---

Github supports todo list by itself. We can simply do following:
> [x] This item is done.
> [] This item is to be done.

[x] This item is done.
[] This needs to be done.

However, in jupyter notebook python (powered by markdown.js) there is no native way to do this.  
But we can use html to get the same result. 

> <input type="checkbox" disabled checked>  This item is checked.
> <input type="checkbox" disabled> This is unchecked.


<input type="checkbox" disabled checked>  This item is checked.
<input type="checkbox" disabled> This is unchecked.
