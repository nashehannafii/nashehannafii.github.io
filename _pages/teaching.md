---
layout: page
permalink: /teaching/
title: Teaching
description: Teaching positions at Universitas Darussalam Gontor — courses in programming, informatics, and statistics.
nav: true
nav_order: 3
---

<!-- pages/teaching.md -->
<div class="teaching">
  <h3>Universitas Darussalam Gontor</h3>
  <p>Lecturer — click a course to open its learning materials page.</p>

{% assign sorted_courses = site.courses | sort: "importance" %}

  <div class="row row-cols-1 row-cols-md-3 mt-2">
    {% for course in sorted_courses %}
      {% include courses.liquid %}
    {% endfor %}
  </div>
</div>
