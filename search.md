---
layout: default
title: Search
---

<form>
  <div>
    <input id="in_Default" type="text" placeholder="Search.." name="search">
  </div>
</form>

<hr/>
<ol style="text-align: left!important;" id="results-container"></ol>

<!-- script pointing to search.js -->
  <script src="{{ site.baseurl }}/assets/js/search.js"></script>

  <script>
  var sjs = SimpleJekyllSearch({
    searchInput: document.getElementById('in_Default'),
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
  padding: 15px;
  font-size: 17px;
  border: none;
  float: none;
  width: 80%;
  background: transparent;
  color: #00ff00;
  border: 2px solid #00ff00;
}

form input[type="text"]:hover {
  border: 2px solid red;
}
</style>
