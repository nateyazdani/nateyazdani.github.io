---
layout: page
permalink: /pubs/
title: research articles
description: publications from my research
navigation: publications
years: [2021, 2019, 2018, 2017]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -q @*[year={{y}}]* %}
{% endfor %}
