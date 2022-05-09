---
layout: page
permalink: /publications/
title: publications
description: A growing collection of the research papers I published.
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
