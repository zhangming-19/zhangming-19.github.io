---
layout: page
permalink: /publications/
title: publications
description: Please see my full publication list at <a href='https://scholar.google.com.hk/citations?user=-QVrM-QAAAAJ'><u>google scholar</u></a>.
years: [2024, 2022, 2021, 2019]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
