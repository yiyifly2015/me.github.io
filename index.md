---
title: "Welcome to My Creative World"
layout: single
permalink: /
---

# 👋 Hello, I’m Kid!

This is my personal site where I share **writing, photos, and videos**.  
Here are my latest creations 👇

---

## ✍️ Latest Writing
{% assign latest_posts = site.posts | sort: "date" | reverse | slice: 0, 3 %}
<ul>
{% for post in latest_posts %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <em>{{ post.date | date: "%Y-%m-%d" }}</em>
  </li>
{% endfor %}
</ul>

👉 More: [Writings](/posts/)

---

## 📸 Latest Photos
<!--
  {% assign latest_photo = site.photos | sort: "date" | last %}
  **[{{ latest_photo.title }}]({{ latest_photo.file }})**
  *{{ latest_photo.date | date: "%Y-%m-%d" }}*  
-->

{% assign latest_photos = site.photos | sort: "date" | reverse | slice: 0, 3 %}
<ul>
{% for photo in latest_photos %}
  <li>
    {{ photo.title }}<br>
    <img src="{{ photo.file }}" alt="{{ photo.title }}" width="300"><br>
    <em>{{ photo.date | date: "%Y-%m-%d" }}</em>
  </li>
{% endfor %}
</ul>

👉 More: [Photos](/photos/)

---

## 🎬 Latest Video
<!--
  {% assign latest_video = site.videos | sort: "date" | last %}
  **{{ latest_video.title }}**
  <iframe width="560" height="315"
        src="https://www.youtube.com/embed/{{ latest_video.youtube_id }}"
        title="YouTube video player"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
        allowfullscreen>
  </iframe>
  *{{ latest_video.date | date: "%Y-%m-%d" }}*
-->
{% assign latest_videos = site.videos | sort: "date" | reverse | slice: 0, 3 %}
<ul>
{% for video in latest_videos %}
  <li>
    {{ video.title }}<br>
    <iframe width="560" height="315"
        src="https://www.youtube.com/embed/{{ latest_video.youtube_id }}"
        title="YouTube video player"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
        allowfullscreen>
    </iframe>
    <em>{{ video.date | date: "%Y-%m-%d" }}</em>
  </li>
{% endfor %}
</ul>

👉 More: [Videos](/videos/)
