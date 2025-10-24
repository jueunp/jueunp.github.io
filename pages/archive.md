
---
layout: default
title: 전체 게시글
permalink: /archive/
---
<h2>전체 게시글</h2>
<div class="archive-list">
  <ul>
  {% assign posts = site.posts | sort: 'date' | reverse %}
  {% for post in posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <small> · {{ post.date | date: "%Y-%m-%d" }} · {{ post.categories | join: ', ' }}</small>
    </li>
  {% endfor %}
  </ul>
</div>
