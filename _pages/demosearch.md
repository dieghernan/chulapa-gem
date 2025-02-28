---
title: Demo search
permalink: /demosearch
---



<form class="input-group">
    <label class="sr-only" for="search"> Search </label>
    <input type="search" id="search-input" class="form-control rounded-right" placeholder="{{ site.search.label | default: "Search" }}...">
</form>
<p class="text-right small mt-1"> Powered by <a href="https://github.com/christian-fei/Simple-Jekyll-Search">Simple-Jekyll-Search</a></p>

<div id="results-container" class="mt-3 text-left"></div>

<script src="{{ 'assets/simple-jekyll-search.min.js' | absolute_url }}" type="text/javascript"></script>

<script>
    SimpleJekyllSearch({
    searchInput: document.getElementById('search-input'),
    resultsContainer: document.getElementById('results-container'),
    searchResultTemplate: '<article class="my-2 text-left"><div class="row"><div class="col"><h5 class="chulapa-links-hover-only" itemprop="headline"><a href="{url}" rel="permalink">{title}</a></h5></div></div><div class="row mt-2"><div class="col"><p>{excerpt}</p></div></div><hr></article>',
    json: '{{ "/assets/search.json" | absolute_url }}' 
    });
</script>