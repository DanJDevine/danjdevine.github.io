---
layout: page
permalink: /progress/
title: works in progress
description: these are ongoing, under review, or with revise and resubmit status.
years: [2023, 2022]
nav: false
order: 3
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f wip -q @*[year={{y}}]* %}
{% endfor %}

</div>
