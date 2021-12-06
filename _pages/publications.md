---
layout: page
permalink: /publications/
title: publications
description: Below you will find a list of my recent publications in academic journals, conference proceedings as well as non-academic outlets.
#Should you fail to access any of the below articles via the linked journal websites, please drop me an email and I will happily send you a copy.
#type_order: [article,inproceedings]
years_articles: [2021,2015]
years_confs: [2021,2020,2019]
years_media: [2021,2020,2019]
#sort_by: type_order, years
order: descending

nav: true #change to true if wanted in nav bar
---

### publications in refereed academic journals

<div class="publications">

{% for y in page.years_articles %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f journal_pubs -q @*[year={{y}}]* %}
{% endfor %}

</div>

### publications in refereed conference proceedings

<div class="publications">

{% for y in page.years_confs %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f conf_pubs -q @*[year={{y}}]* %}
{% endfor %}

</div>

### technical reports and publications in media outlets

<div class="publications">

{% for y in page.years_media %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f media_pubs -q @*[year={{y}}]* %}
{% endfor %}

</div>
