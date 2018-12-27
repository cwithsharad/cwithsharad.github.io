---
layout: blog
title: Search
---

<div class="jumbotron" style="background:rgb(0,0,0,0.8)!important">
 <div class="input-group input-group-lg">
  <input type="text" class="form-control" id="inputDefault" placeholder="Search..." aria-describedby="sizing-addon1">
</div> 
<ol id="results-container">
<ol>
</div>
 

  <!-- script pointing to search.js -->
  <script src="{{ site.baseurl }}/assets/js/search.js"></script>

  <script>
  var sjs = SimpleJekyllSearch({
    searchInput: document.getElementById('inputDefault'),
    resultsContainer: document.getElementById('results-container'),
    json: '{{ site.baseurl }}/search.json'
  })
  </script>
