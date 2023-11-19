---
layout: page
permalink: /publications/
title: publications
description: Our research interests are mainly on designing novel solutions and employing various applied mathematical tools (i.e., stochastic modeling, queueing theory and optimization theory) and machine learning techniques to design, analyze and optimize the cutting-edge applications in complex wire/wireless networks: fog/edge computing and data center, IoT networks, 5G/6G network resource allocations, distributed machine learning for wireless networks, and wireless sensing/imaging. An updated list of all published papers including refereed and non-refereed ones is available from <a href='https://scholar.google.com/citations?user=wgsX_zIAAAAJ&hl=en'>Google Scholar</a> 
years: [2023, 2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014]
nav: true
nav_order: 3
---


<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
