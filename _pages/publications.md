---
layout: page
permalink: /publications/
title: Publications
description:  
years: [2021, 2020, 2018, 2017, 2016, 2015, 2014]
nav: true
---

You can find below a list of my publications by categories (preprint, international journal and conference proceedings, thesis) and in reversed chronological order.

## Preprint

<div class="publications">

{% bibliography --file mchampion_preprint %}

</div>

## International journal and conference proceedings

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f mchampion_journal -q @*[year={{y}}]* %}
{% endfor %}


</div>


## Thesis

<div class="publications">

{% bibliography --file mchampion_thesis %}

</div>

