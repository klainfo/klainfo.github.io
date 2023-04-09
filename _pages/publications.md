---
layout: page
permalink: /publications/
title: publications
description: >
  In my research area of Software Engineering (SE), it is common to publish completed research in top-tier conferences as full-length, peer-reviewed papers (10-12 pages). The top SE conferences have very low acceptance rates (<30%) and a few are even considered more prestigious, having significantly more impact and citations, than most journals. The author's order is generally based on the contribution to the publication. In the case of PhD student projects, the convention is to have the PhD student as the first author, where I will be a corresponding author in the second or third author's order.

years: [2023, 2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014, 2013]
nav: true
nav_order: 4
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
</div>
