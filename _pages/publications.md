---
layout: page
permalink: /publications/
title: Publications 
description: <p  style="position:relative; top:-3.5rem"> For the full list refer to my google-scholar page <a href="https://scholar.google.com/citations?user=7V-JmgIAAAAJ" target="_blank" title="Google Scholar" style="font-size:40px; position:relative; top:+7px"><i  class="ai ai-google-scholar"></i></a> </p>
years: [2022,2021]
nav: true
---


<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
