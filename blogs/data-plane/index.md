---
layout: default
title: Data Plane Blogs
permalink: /blogs/data-plane/
---

# Data Plane Blogs

Explore all Data Plane, VPP, and DPDK blog posts:

<div class="section-divider"></div>

<div class="projects-list" style="display:flex;flex-wrap:wrap;gap:2rem 2.5rem;justify-content:center;">
{% assign dp_posts = site.posts | where_exp: "post", "post.categories contains 'data-plane' or post.categories contains 'vpp' or post.categories contains 'dpdk'" %}
{% for post in dp_posts %}
  <div class="project-card" style="min-width:240px;max-width:320px;background:rgba(255,255,255,0.92);border-radius:14px;box-shadow:0 2px 12px #e2e8f0;padding:1.3rem 1.1rem;text-align:center;transition:box-shadow 0.2s;position:relative;overflow:hidden;">
    <span style="font-size:2.1rem;">🌐</span>
    <h3 style="margin:0.8rem 0 0.3rem 0;font-size:1.18rem;font-weight:700;">
      <a href="{{ post.url | relative_url }}" style="color:#1976d2;text-decoration:none;">{{ post.title }}</a>
    </h3>
    <div style="color:#607d8b;font-size:0.98rem;margin-bottom:0.5rem;">{{ post.date | date: "%B %d, %Y" }}</div>
    <div style="color:#455a64;font-size:0.97rem;">{{ post.excerpt | strip_html | truncate: 90 }}</div>
  </div>
{% endfor %}
</div>
  {% endif %}
{% endfor %}
</div>
