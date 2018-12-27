---
layout: page
title: Search
---

<form class="bs-component">
                    <div class="form-group">
                        <input class="form-control" id="focusedInput" placeholder="Search... type="text">
                    </div>
</form>	

<ol id="results-container">
<ol>


  <!-- script pointing to search.js -->
  <script src="{{ site.baseurl }}/assets/js/search.js"></script>

  <script>
  var sjs = SimpleJekyllSearch({
    searchInput: document.getElementById('focusedInput'),
    resultsContainer: document.getElementById('results-container'),
    json: '{{ site.baseurl }}/search.json'
  })
  </script>
