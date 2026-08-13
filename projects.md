---
layout: default
title: Projects
---

# Projects

Here are some of the projects I've worked on.

{% for project in site.projects %}

## [{{ project.title }}]({{ project.url | relative_url }})

{{ project.description }}

{% endfor %}
