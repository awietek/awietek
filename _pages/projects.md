---
layout: page
title: Research
permalink: /projects/
description: An overview over my current and past research.
nav: true
order: 1
---


{% assign sorted_projects = site.projects | sort: "importance" %}
{% for project in sorted_projects %}

<div class="table">
{% if project.img %}

<img width=220px src="{{ project.img | relative_url }}" alt="project thumbnail" align=left style="margin:15px;">

{% endif %}

<h2 class="card-title">{{ project.title }}</h2>
{% if project.descriptionfront %}
<p class="card-text">{{ project.descriptionfront }}</p>
{% else %}
<p class="card-text">{{ project.description }}</p>
{% endif %}
<a href="{{ project.url | relative_url }}"> Read more </a>
</div>
<hr>

{% endfor %}


