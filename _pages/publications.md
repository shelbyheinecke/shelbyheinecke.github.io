---
layout: page
permalink: /publications/
title: publications
description: Works with * indicate alphabetical ordering of authors.
years: [2022, 2021, 2020, 2019, 2018, In Preparation]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
