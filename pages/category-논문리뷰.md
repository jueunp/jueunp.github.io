
---
layout: default
title: 논문리뷰
permalink: /category/%EB%85%BC%EB%AC%B8%EB%A6%AC%EB%B7%B0/
---
<h2>논문리뷰</h2>
<ul>
{% for post in site.posts %}
  {% if post.categories contains "논문리뷰" %}
    <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a> <small>{{ post.date | date: "%Y-%m-%d" }}</small></li>
  {% endif %}
{% endfor %}
</ul>
