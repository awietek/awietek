---
layout: page
permalink: /publications/
title: Publications
description: #publications by categories in reversed chronological order
years: [2020, 2019, 2018, 2017, 2016, 2015]
nav: true
order : 2
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
