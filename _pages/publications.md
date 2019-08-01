---
layout: page
permalink: /publications/
title: publications
description: Below is a collection of my published works. For the most up-to-date version of my published works, please refer to my [Google Scholar Profile](https://scholar.google.ca/citations?user=L0E4foIAAAAJ&hl=en).
years: [1956, 1950, 1935, 1905]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
