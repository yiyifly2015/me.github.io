---
title: "Photos"
layout: single
permalink: /photos/
---

# 📸 My Photo Albums

Choose an album:

<ul>
{% assign grouped = site.photos | group_by: "category" %}
{% for group in grouped %}
  <li><a href="/photos/{{ group.name }}/">{{ group.name | capitalize }}</a></li>
{% endfor %}
</ul>

