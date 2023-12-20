---
layout: page
permalink: /publications/
title: academic publications
description: These are all published work. For unpublished work, see the works in progress tab. 
years: [2023, 2022, 2021, 2020, 2019]
nav: false
nav_order: 3
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
