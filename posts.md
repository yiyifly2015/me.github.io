---
title: "Writing"
layout: single
permalink: /posts/
---

# ✍️ My Writing

Here are some of my selected works:

<ul>
{% assign grouped = site.posts | group_by: "category" %}
{% for group in grouped %}
  <li>📖<a href="/posts/{{ group.name }}/">{{ group.name | capitalize }}</a></li>
{% endfor %}
</ul>

