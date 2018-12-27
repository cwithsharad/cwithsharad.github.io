---
layout: blog
title: Search
---

<div class="col-lg-12">
                <form class="bs-component">
                    <div class="form-group">
                        <input class="form-control" id="focusedInput" placeholder="Search... type="text">
                    </div>
                </form>	
</div>
                                                                                                        
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







 <div class="row">
           <div class="col-lg-12 col-lg-offset-1">
                <form class="bs-component">
                    <div class="form-group">
                        <label class="control-label" for="focusedInput">Focused input</label>
                        <input class="form-control" id="focusedInput" value="This is focused..." type="text">
                    </div>
                    <div class="form-group">
                        <label class="control-label" for="disabledInput">Disabled input</label>
              <input class="form-control" id="disabledInput" placeholder="Disabled input here..." disabled="" type="text">
                    </div>
                    <div class="form-group has-warning">
                        <label class="control-label" for="inputWarning">Input warning</label>
                        <input class="form-control" id="inputWarning" type="text">
                    </div>
                    <div class="form-group has-error">
                        <label class="control-label" for="inputError">Input error</label>
                        <input class="form-control" id="inputError" type="text">
                    </div>
                    <div class="form-group has-success">
                        <label class="control-label" for="inputSuccess">Input success</label>
                        <input class="form-control" id="inputSuccess" type="text">
                    </div>
                    <div class="form-group">
                        <label class="control-label" for="inputLarge">Large input</label>
                        <input class="form-control input-lg" id="inputLarge" type="text">
                    </div>
                    <div class="form-group">
                        <label class="control-label" for="inputDefault">Default input</label>
                        <input class="form-control" id="inputDefault" type="text">
                    </div>
                    <div class="form-group">
                        <label class="control-label" for="inputSmall">Small input</label>
                        <input class="form-control input-sm" id="inputSmall" type="text">
                    </div>
                    <div class="form-group">
                        <label class="control-label">Input addons</label>
                        <div class="input-group">
                            <span class="input-group-addon">$</span>
                            <input class="form-control" type="text">
                            <span class="input-group-btn">
                                <button class="btn btn-default" type="button">Button</button>
                            </span>
                        </div>
                    </div>
                </form>
            </div>
        </div>
