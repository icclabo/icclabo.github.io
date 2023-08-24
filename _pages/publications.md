---
layout: page
permalink: /publications/
title: publications
description: An updated list of all published papers including refereed and non-refereed ones is available from <a href='https://scholar.google.com/citations?user=wgsX_zIAAAAJ&hl=en'>Google Scholar</a> 
types: [Journals, Conferences, Book Chapters]
nav: true
nav_order: 3
---


<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.types %}
  <h2 class="journal">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}



</div>
