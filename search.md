---
layout: default
title: Search
---

<form>
  <div>
    <input id="inputDefault" type="text" placeholder="Search.." name="search">
  </div>
</form>

<hr/>
<ol style="text-align: left!important;" id="results-container"></ol>

<!-- script pointing to search.js -->
  <script src="{{ site.baseurl }}/assets/js/search.js"></script>

  <script>
  var sjs = SimpleJekyllSearch({
    searchInput: document.getElementById('inputDefault'),
    resultsContainer: document.getElementById('results-container'),
    json: '{{ site.baseurl }}/search.json'
  })
</script>




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
