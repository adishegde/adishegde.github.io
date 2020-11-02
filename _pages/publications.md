---
layout: page
permalink: /publications/
title: Publications
description: A list of publications in reverse chronological order.
years: [2020]
nav: true
---

<p>
Authors are primarily listed in alphabetical order which is the norm in cryptography and theoretical CS. In some cases, an asterisk (*) is used to indicate equal contribution and lead authorship.
</p>

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
