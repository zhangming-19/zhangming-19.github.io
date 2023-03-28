---
layout: page
permalink: /publications/
title: publications
description: Please see my full publication list at <a href='https://scholar.google.com/citations?hl=en&user=pmjB_ZQAAAAJ'><u>google scholar</u></a> or <a href='https://www.semanticscholar.org/author/2072592545'><u>semantic scholar</u></a>.
years: [2023, 2022, 2021, 2019]
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
