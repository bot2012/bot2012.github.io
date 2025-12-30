---
layout: page
title: Projects
permalink: /projects/
---

{% for project in site.projects %}
### [{{ project.title }}]({{ project.url }})
**Tech:** {{ project.tech }}

{{ project.excerpt }}
{% endfor %}