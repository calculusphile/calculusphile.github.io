---
layout: default
title: Home
---

# 👋 Welcome to Calculusphile

My personal hub for projects, blogs, and learning resources in programming and Computer Science & Engineering.


## 🚀 Latest Projects

<div class="projects-list">
    {% for project in site.projects limit: 3 %}
    <div class="project-card">
        <h3><a href="{{ project.url }}">{{ project.title }}</a></h3>
        {% if project.description %}
            <p>{{ project.description }}</p>
        {% endif %}
    </div>
    {% endfor %}
</div>


[View All Projects →]({{ '/projects' | relative_url }})


## 📝 Latest Blog Posts

{% for post in site.posts limit: 3 %}
- **[{{ post.title }}]({{ post.url }})** - <time>{{ post.date | date: "%B %d, %Y" }}</time>
{% endfor %}

[Read More Posts →]({{ '/blog' | relative_url }})


## 💡 About This Site

This portfolio showcases my journey in programming, learning data structures & Algorithm during my Computer Science Engineering. Feel free to explore my work and [learn more about me]({{ '/about' | relative_url }}).
