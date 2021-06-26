---
layout: page
permalink: /publications/
title: publications
description: Here is a list of my publications. PDFs are linked if available, otherwise please feel free to email me for a copy.
years: [2021]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
