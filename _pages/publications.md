---
layout: page
permalink: /publications/
title: Publications
description: 
years: [2024, 2019]
years1: [2021, 2016]
years2: [2023,2022,2017]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>

<h1 class="post-title">Contributed Talks</h1>
<div class="publications">

{%- for y in page.years1 %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f talks -q @*[year={{y}}]* %} 
{% endfor %}

</div>

<h1 class="post-title">Selected Posters</h1>
<div class="publications">

{%- for y in page.years2 %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f posters -q @*[year={{y}}]* %} 
{% endfor %}

</div>
