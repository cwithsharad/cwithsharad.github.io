---
layout: default
title: Search
---

<form>
  <div>
    <input type="text">
    <input type="submit" value="Search">
  </div>
</form>

<style>
/*
First, we set the `box-sizing` value as `border-box` so ...
we could easily expand this element to 100% width without worrying about
the `padding` and `border-width` calculation.
*/

form input {box-sizing:border-box}


/*
create the room for the button using `margin`
*/

form > div {
  position:relative;
  margin-right:110px; /* same with `button width` + `button distance from search field` */
}


/*
SEARCH FIELD: the `box-sizing` value for this element already set as `border-box`
and the right margin value also already set with the correct value
to make the room for the button, so now we could safely
expand this element to 100% width!
*/

form input[type="text"] {
  display:block;
  width:100%;
}
</style>
