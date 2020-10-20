---
layout: page
permalink: /publications/
title: Publications
description: 
years: [2020, 2019, 2018, 2017, 2014]
yearsj: [2014]
yearsm: [2020]
nav: true
---

<h3>Conference Papers</h3>

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>

<br>
<h3>Journal Papers</h3>

<div class="publications">
{% for y in page.yearsj %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f journal -q @*[year={{y}}]* %}
{% endfor %}
</div>

<br>
<h3>Manuscripts</h3>
<div class="publications">
{% for yy in page.yearsm %}
  <h2 class="year">{{yy}}</h2>
  {% bibliography -f manuscripts -q @*[year={{yy}}]* %}
{% endfor %}
</div>




