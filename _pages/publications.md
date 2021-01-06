---
layout: page
permalink: /publications/
title: Selected Publications
years: [2015, 2014, 2012, 2011, 2010]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
