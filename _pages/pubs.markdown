---
layout: page
permalink: /pubs/
title: publications
description: Publications in reverse chronological order.
years: [2018, 2017]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -q @*[year={{y}}]* %}
{% endfor %}
