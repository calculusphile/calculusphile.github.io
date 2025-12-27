---
layout: default
title: Competitive Programming Blogs
permalink: /blogs/competitive-programming/
---

# Competitive Programming Blogs

Explore all Competitive Programming and Problem Solving blog posts:

{% assign cp_posts = site.posts | where_exp: "post", "post.categories contains 'competitive-programming' or post.categories contains 'problem-solving'" %}
{% for post in cp_posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) <small>{{ post.date | date: "%B %d, %Y" }}</small>
{% endfor %}
