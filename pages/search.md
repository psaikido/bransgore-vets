---
layout: page
title: Search
url: pages/search/
permalink: search
---

<div id="search">
    <div class="uk-background-default uk-border-rounded">
        <form class="uk-search uk-search-navbar uk-width-1-1" onsubmit="return false;">
            <input id="navbar-search" class="uk-search-input" type="search" placeholder="Search..." autofocus>
        </form>
        <ul id="navbar-search-results" class="uk-position-absolute uk-width-1-1 uk-list"></ul>
    </div>
</div>

<script>
SimpleJekyllSearch({
    searchInput: document.getElementById('navbar-search'),
    resultsContainer: document.getElementById('navbar-search-results'),
    noResultsText: '<li>No results found</li>',
    searchResultTemplate: '<li><a href="{url}">{title}</a></li>',
    json: '{{ "search.json" | abolute_url }}'
});
</script>
