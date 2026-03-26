---
layout: page
title: Projects
permalink: /projects/
description: A growing collection of my projects.
nav: true
nav_order: 3
horizontal: false
---

<!-- pages/projects.md -->
<div class="projects">

{% assign sorted_projects = site.projects | where_exp: "project", "project.hidden != true" | sort: "importance" %}

{% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
{% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
{% endif %}

</div>
