---
layout: post
title: Using Snippet Editor in Safari
---

Date: Sep 15, 2018  

When we are using Safari browser, if we want to run some quick `html` or `javascript` code, we can simply open the
Snippet Editor from the menu `Develop > Show Snippet Editor`.

Example html:
```
<style>
.myclass{
    font-weight: bold;
    font-family: Verdana;
    font-size: 1.3em;
}
</style>
<div class=myclass>This is an example sentence.</div>
```



Example JavaScript:
```
<script>

// hello world
document.write("Hello, world!");
document.write("<br>")

// adding variables
var a = 5;
var b = 3;
document.write("sum of a and b = ", a+b);

//for loop example
for (var i=0; i<10;i++){
    document.write(i + "<br>");
}
</script>
```



