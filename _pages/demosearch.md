---
title: Demo search
permalink: /demosearch
---


<div id="search-container">
    <input type="text" id="search-input" placeholder="Search through the blog posts...">
    <ul id="results-container"></ul>
</div>

<script src="{{ 'assets/simple-jekyll-search.min.js' | absolute_url }}" type="text/javascript"></script>

<script>
    SimpleJekyllSearch({
    searchInput: document.getElementById('search-input'),
    resultsContainer: document.getElementById('results-container'),
    searchResultTemplate:                     '<article class="my-2 text-left">' 	+
                    '<div class="row">'	+
                    '<div class="col">' +
                    '<h5 class="chulapa-links-hover-only" itemprop="headline">' +
                    '<a href="{url}" rel="permalink">{title}</a>' +
                    '</h5>' +
                    '</div>'		+
                    '</div>'		+
                    '<div class="row mt-2">' +
                    '<div class="col">' +
                    '<p>{excerpt}</p>' +
					'</div>' +
					'</div>' +
					'<hr>' +
					'</article>';,
    json: '{{ "search.json" | absolute_url }}' 
    });
</script>