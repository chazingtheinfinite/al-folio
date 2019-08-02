---
layout: page
permalink: /publications/
title: publications
description: Below is a collection of my published works. For the most up-to-date version of my published works, please refer to my <a href="https://scholar.google.ca/citations?user=L0E4foIAAAAJ&hl=en"><b>Google scholar Profile</b></a>.
years: [2019, 2018, 2017, 2016, 2015, 2014, 2013, 2012, 2011, 2010, 2009, 2008, 2007, 2006, 2005, 2004, 2003, 2002, 2001, 2000, 1999, 1998, 1997, 1996]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
