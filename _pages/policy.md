---
layout: page
permalink: /policy/
title: policy publications
description: These are policy-related outputs.
years: [2022, 2021, 2020, 2019, 2017, 2016]
nav: false
nav_order: 3
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f polpapers -q @*[year={{y}}]* %}
{% endfor %}

</div>
