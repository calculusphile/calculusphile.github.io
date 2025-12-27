---
layout: default
title: Competitive Programming Blogs
permalink: /blogs/competitive-programming/
---

# Competitive Programming Blogs

Explore all Competitive Programming and Problem Solving blog posts:

<div class="projects-list" style="display:flex;flex-wrap:wrap;gap:2rem 2.5rem;justify-content:center;">
{% for post in site.posts %}
  {% if post.categories contains 'competitive-programming' or post.categories contains 'problem-solving' %}
    <div class="project-card" style="min-width:240px;max-width:320px;background:#f8fafc;border-radius:10px;box-shadow:0 2px 8px #e2e8f0;padding:1.2rem 1rem;text-align:center;">
      <span style="font-size:2rem;">🏆</span>
      <h3 style="margin:0.7rem 0 0.3rem 0;font-size:1.18rem;font-weight:700;">
        <a href="{{ post.url | relative_url }}" style="color:#1976d2;text-decoration:none;">{{ post.title }}</a>
      </h3>
      <div style="color:#607d8b;font-size:0.98rem;margin-bottom:0.5rem;">{{ post.date | date: "%B %d, %Y" }}</div>
      <div style="color:#455a64;font-size:0.97rem;">{{ post.excerpt | strip_html | truncate: 90 }}</div>
    </div>
  {% endif %}
{% endfor %}
</div>
