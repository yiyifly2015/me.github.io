---
title: "Videos"
layout: single
permalink: /videos/
---

# 🎬 My Videos

Choose a category:

<ul>
{% assign grouped = site.videos | group_by: "category" %}
{% for group in grouped %}
  <li><a href="/videos/{{ group.name }}/">{{ group.name | capitalize }}</a></li>
{% endfor %}
</ul>
