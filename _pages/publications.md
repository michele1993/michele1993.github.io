---
layout: page
permalink: /publications/
title: Publications
description: 
years: [2023, 2022, 2019]
years1: [2021, 2014]
years2: [2021]
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

<h1 class="post-title">Contributed Talks</h1>
<div class="publications">

{%- for y in page.years1 %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f talks -q @*[year={{y}}]* %} 
{% endfor %}

</div>

</div>
<h1 class="post-title">Selected Posters</h1>
<div class="publications">

{%- for y in page.years2 %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f posters -q @*[year={{y}}]* %} 
{% endfor %}

</div>
