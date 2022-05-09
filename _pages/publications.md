---
layout: page
permalink: /publications/
title: publications
description: See more on [my Google Scholar](https://scholar.google.com/citations?user=EbtrluQAAAAJ&hl=en&authuser=3).
years: [2017, 2018, 2019, 2021]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
