---
layout: default
title: Algorithms
permalink: /blogs/algorithms/
---

# Algorithms Blogs

{% assign posts = site.posts | where_exp: "p", "p.categories contains 'algorithms'" %}

{% for post in posts %}
- [{{ post.title }}]({{ post.url | relative_url }})  
  <small>{{ post.date | date: "%B %d, %Y" }}</small>
{% endfor %}
