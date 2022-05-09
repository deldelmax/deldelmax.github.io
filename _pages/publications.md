---
layout: page
permalink: /publications/
title: publications
description: A growing collection of the research papers I published. Also see my Google Scholar <a href="https://scholar.google.com/citations?user=EbtrluQAAAAJ&hl=en&authuser=3">profile</a>.
years: [2021, 2019, 2018, 2017]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
