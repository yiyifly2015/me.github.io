---
title: "Creative Map"
layout: single
permalink: /map/
---

# 🗺️ Creative Map

Welcome to my personal museum of creations!  
Explore different areas of my work 👇

---

## ✍️ Writing
<ul>
  <li>
    <a href="/posts">All Posts</a>
  </li>
{% assign grouped_posts = site.posts | group_by_exp: "post", "post.categories | first" %}
{% for group in grouped_posts %}
  <li><a href="/posts/{{ group.name }}/">{{ group.name | capitalize }}</a></li>
{% endfor %}
</ul>

---

## 📸 Photos
<ul>
  <li>
    <a href="/photos">All Photos</a>
  </li>
{% assign grouped_photos = site.photos | group_by: "category" %}
{% for group in grouped_photos %}
  <li><a href="/photos/{{ group.name }}/">{{ group.name | capitalize }}</a></li>
{% endfor %}
</ul>

---

## 🎬 Videos
<ul>
  <li>
    <a href="/videos">All Videos</a>
  </li>
{% assign grouped_videos = site.videos | group_by: "category" %}
{% for group in grouped_videos %}
  <li><a href="/videos/{{ group.name }}/">{{ group.name | capitalize }}</a></li>
{% endfor %}
</ul>

---

## 🏠 Back Home
- [Home](/)
- [About Me](/about/)

