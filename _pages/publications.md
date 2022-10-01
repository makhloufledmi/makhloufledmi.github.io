---
layout: page
permalink: /publications/
title: Publications
description:  
years: [2022, 2021, 2020, 2019]
nav: true
---

You can find below a list of my publications by categories (preprint, international journal, conference proceedings and thesis) and in reversed chronological order.

## Preprint

<div class="publications">

{% bibliography --file mchampion_preprint %}

</div>

## International journal

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f mchampion_journal -q @*[year={{y}}]* %}
{% endfor %}


</div>

## Conference proceedings

<div class="publications">

{% bibliography --file mchampion_proc %}


</div>

## Thesis

<div class="publications">

{% bibliography --file mchampion_thesis %}

</div>

