
---
layout: default
title: #diffusion
permalink: /tag/diffusion
---
<h2>#diffusion</h2>
<ul>
{% for post in site.tags.diffusion %}
  <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a> <small>{{ post.date | date: "%Y-%m-%d" }}</small></li>
{% endfor %}
</ul>
