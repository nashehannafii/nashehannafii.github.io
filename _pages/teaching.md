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
  <p class="mb-3">
    <span class="badge mr-1" style="background: #ffedd5; color: #c2410c;">PROGRAMMING</span>
    <span class="badge mr-1" style="background: #ccfbf1; color: #0f766e;">CONCEPT</span>
    <span class="badge" style="background: #fce7f3; color: #be185d;">MATH</span>
  </p>

{% assign sorted_courses = site.courses | sort: "importance" %}

  <div class="row row-cols-1 row-cols-md-3">
    {% for course in sorted_courses %}
      {% include courses.liquid %}
    {% endfor %}
  </div>
</div>
