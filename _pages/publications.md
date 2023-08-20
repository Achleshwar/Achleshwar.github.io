---
layout: page
permalink: /publications/
title: Publications
description: Selected papers in reversed chronological order. Please visit my google scholar page for a complete list of publications.
years: [2023, 2022, 2021]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
