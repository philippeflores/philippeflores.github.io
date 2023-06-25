---
layout: page
permalink: /publications/
title: publications
description: Please do not hesitate to contact me by e-mail if you want to discuss on any of my publications.
years: [2022, 2023]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
