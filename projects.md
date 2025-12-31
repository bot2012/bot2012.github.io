---
layout: page
title: Projects
permalink: /projects/
---
<!--

{% for project in site.projects %}
### [{{ project.title }}]({{ project.url }})
**Tech:** {{ project.tech }}

{{ project.excerpt }}
{% endfor %}
-->

<!-- 
    Coverting projects into cards. 
-->

<div class="project-grid">
{% for project in site.projects %}
  <div class="project-card">
    <h3>
      <a href="{{ project.url }}">
        {{ project.title }}
      </a>
    </h3>

    <p>{{ project.excerpt }}</p>

    <p class="tech">
      {{ project.tech }}
    </p>
  </div>
{% endfor %}
</div>