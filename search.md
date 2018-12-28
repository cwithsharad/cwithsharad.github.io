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
input:focus, textarea:focus {
    outline: none;
}

form input {box-sizing:border-box}

form > div {
  position:relative;
}

form input[type="text"] {
  padding: 15px;
  font-size: 17px;
  float: none;
  width: 100%;
  background: transparent;
  color: #00ff00;
  border: 2px solid #00ff00;
}

form input[type="text"]:hover {
  border: 2px solid red;
}
</style>
