---
layout: page
permalink: /publications/
title: Publications
description: Authors are listed in alphabetical order which is the norm in cryptography and theoretical CS. In case of exceptions, an asterisk (*) is used to indicate equal contribution and lead authorship.
years: [2020]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
