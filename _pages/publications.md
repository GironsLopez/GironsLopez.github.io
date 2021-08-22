---
layout: page
permalink: /publications/
title: publications
description: Peer-reviewed publications, theses and conference contributions
years: [2021, 2020, 2019, 2018, 2017, 2016, 2015, 2013, 2011]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
