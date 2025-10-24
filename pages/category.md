
---
layout: default
title: 카테고리
permalink: /category/
---
<h2>카테고리</h2>
<ul>
{% assign cats = site.posts | map: 'categories' | join: ',' | split: ',' | uniq | sort %}
{% for c in cats %}
  {% if c != '' %}
  <li><a href="{{ '/category/' | append: c | relative_url }}">{{ c }}</a></li>
  {% endif %}
{% endfor %}
</ul>
