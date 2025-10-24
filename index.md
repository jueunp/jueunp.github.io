
---
layout: default
title: Home
---
<section>
  <h2>최근 글</h2>
  <div class="archive-list">
    <ul>
    {% for post in site.posts limit:10 %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <small> · {{ post.date | date: "%Y-%m-%d" }}</small>
      </li>
    {% endfor %}
    </ul>
  </div>
</section>
