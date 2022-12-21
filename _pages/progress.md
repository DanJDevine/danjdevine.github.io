---
layout: page
permalink: /works in progress/
title: works in progress
description: for resubmitted, under contract, or ongoing projects
years: [ongoing, 2022]
nav: true
order: 3
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f wip -q @*[year={{y}}]* %}
{% endfor %}

</div>
