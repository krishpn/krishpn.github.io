---
layout: page
permalink: /publications/
title: publications
description: selected publications
nav: true
nav_order: 4
---



<div class="publications">

{% if site.bib_search %}
  {% include bib_search.liquid %}
{% endif %}

{% bibliography %}

</div>