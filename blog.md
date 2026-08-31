---
layout: project
title: "Blog"
permalink: /blog/
---

<p class="project-label">Writing · Cyber Security &amp; Digital Forensics</p>

<h1>Blog</h1>

{% for post in site.posts %}

<h2>
  <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
</h2>

<p class="project-post-date">
  {{ post.date | date: "%B %d, %Y" }}
</p>

<p>
  {{ post.excerpt | strip_html | truncatewords: 30 }}
</p>

{% endfor %}
