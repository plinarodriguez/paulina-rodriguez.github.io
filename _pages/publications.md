---
layout: page
permalink: /publications/
title: publications
description: A growing collection of my publications.
years: [2026,2025,2024,2023,2022,2019,2018,2011,2010]
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
