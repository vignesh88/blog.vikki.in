---
layout: default
title: Search
permalink: /search/
---
<h1 class="post-title">Search here</h1>

<div id="search-container">
<input type="text" id="search-input" placeholder="Linux, Kubernetes, photo...">
<ul id="results-container"></ul>
</div>

<style>
#search-container {
    max-width: 100%;
}

input[type=text] {

    outline: none;
    padding: 15px 25px;
    margin: 5px 1px 3px 0px;
    border: none;
    width: 100%;
    border-radius: 1px;
    box-shadow: 0 1px 0px 0 rgba(0,0,0,0.16), 0 0 0 1px rgba(0,0,0,0.08);

}

input[type=text]:hover {
    outline: none;
    border: none;
    margin: 5px 1px 3px 0px;
    padding: 15px 25px;
    -webkit-transition: all 0.30s ease-in-out;
    -moz-transition: all 0.30s ease-in-out;
    -ms-transition: all 0.30s ease-in-out;
    -o-transition: all 0.30s ease-in-out;
     box-shadow: 0 2px 2px 0 rgba(0,0,0,0.16), 0 0 0 1px rgba(0,0,0,0.08);
}

input[type=text]:focus {
    box-shadow: 0 2px 2px 0 rgba(0,0,0,0.16), 0 0 0 1px rgba(0,0,0,0.08);
    margin: 5px 1px 3px 0px;
    padding: 15px 25px;
    border: none;
    outline: none;
        -webkit-transition: all 0.30s ease-in-out;
    -moz-transition: all 0.30s ease-in-out;
    -ms-transition: all 0.30s ease-in-out;
    -o-transition: all 0.30s ease-in-out;
}

@media screen and (max-width: 600px) {
    input[type=text]{
            width: 100%;
            box-sizing: border-box;
    }
    }
</style>

<!-- Script pointing to search-script.js -->
<script src="/assets/js/search.js" type="text/javascript"></script>

<!-- Configuration -->
<script>
SimpleJekyllSearch({
  searchInput: document.getElementById('search-input'),
  resultsContainer: document.getElementById('results-container'),
  json: '/search.json'
})
</script>