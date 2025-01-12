# Introduction

# How to add CSS to HTML. 
CSS is a styling language that is applicable to markup languages like HTML.
There are 3 (and 4th) ways we can add CSS to our HTML documents.

Check the [index.html](index.html) code for a live example.

1. Add to the header as a reference to a CSS file. This is the best pattern to follow, it separates the styles from markup.
```html
<link rel="stylesheet" media="screen" href="main.css">
```
2. Add to the header inside a style tag. (Anti pattern, should be avoided in prod.) 
``` html
<style>
    /*
      In production code style tag should never be used and CSS should moved to an external file. This is only for demo
      and teaching purposes.
     */
    div {
      background-color: aliceblue;
    }
</style>
```
3. Add as a property to an HTML tag. (Anti pattern, should be avoided in prod.)
```html
<div style="margin-top: 20px;">Footer</div>
```
4. Use an `@import` statement within CSS space to include another CSS file. (Anti pattern, should be avoided in prod.)
```css
@import url("footer.css");
```
> Note: Imports must be the first statement in CSS otherwise it will not work!



---
[Go back to ToC](../README.md)
