---
title: Search
layout: page
---

<div id="search-input">
<input type="text" id="search-input" placeholder="Search blog posts..">
<ul id="results-container"></ul>
</div>

<script src="{{ site.url }}/assets/js/simple-jekyll-search.min.js" type="text/javascript"></script>

<script>
SimpleJekyllSearch({
    searchInput: document.getElementById('search-input'),
    resultsContainer: document.getElementById('results-container'),
    json: '{{ site.baseurl }}/search.json',
    searchResultTemplate: '<li><div><a href="{url}"><h4>{title}</h4></a><aside>{date}</aside></div></li>',
    noResultsText: 'No results found',
    limit: 10,
    fuzzy: false,
    exclude: ['Welcome']
})
</script>