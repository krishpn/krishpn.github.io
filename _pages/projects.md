---
layout: page
title: Research and analysis
permalink: /projects/
nav: true
nav_order: 3
---

<div class="projects">
  {% assign categories = "work, fun" | split: ", " %}
  {% for category in categories %}
    <h2 class="category">{{ category }}</h2>
    {% assign categorized_projects = site.projects | where: "category", category %}
    <div class="container">
      <div class="row row-cols-1 row-cols-md-3">
        {% for project in categorized_projects %}
          {% include projects.liquid %}
        {% endfor %}
      </div>
    </div>
  {% endfor %}
</div>