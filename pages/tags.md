
---
layout: default
title: Tags
permalink: /tags/
---
<h2>Tags</h2>
<ul>
{% assign all_tags = site.tags %}
{% for tag in all_tags %}
  <li><a href="{{ '/tag/' | append: tag[0] | relative_url }}">#{{ tag[0] }}</a> ({{ tag[1].size }})</li>
{% endfor %}
</ul>
