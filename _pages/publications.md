---
layout: page
permalink: /publications/
title: publications
description: An updated list of all published papers including refereed and non-refereed ones is available from <a href='https://scholar.google.com/citations?user=wgsX_zIAAAAJ&hl=en'>Google Scholar</a> 
years: [2023, 2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014]
nav: true
nav_order: 3
---



<!-- _pages/publications.md -->
<div class="publications">

<h2>Journal Articles</h2>
{% for post in bibliography.papers reversed %}
  {% if post.pubtype == 'journal' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}

<h2>Conference Papers</h2>
{% for post in bibliography.papers reversed %}
  {% if post.pubtype == 'conference' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}

<h2>Book/Book Chapters</h2>
{% for post in bibliography.papers reversed %}
  {% if post.pubtype == 'book' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}
</div>
