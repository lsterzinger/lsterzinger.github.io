---
layout: page
permalink: /publications/
title: Publications
description: Here is a list of my publications. PDFs are linked if available, otherwise please feel free to email me for a copy.
years: [2022, 2021]
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
