---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: Home
---

<!--
# Hi, I am Benson Osei Tutu (Bot)  
I am learning and growing in analytics, data science, and machine learning through hands-on projects and collaboration. This portfolio documents what I am exploring, building, and reflecting on as I continue to develop my skills.

Open to data analytics, science and engineering roles.

Contact: | boseitutu2009@gmail.com | bo2427a@american.edu

-->

# Featured Projects 
<!--
{% assign featured_projects = site.projects | where: "featured", true %}

{% for project in featured_projects %}
### [{{ project.title }}]({{ project.url }})

**Tech:** {{ project.tech }}

{{ project.excerpt }}

{% endfor %}
-->
<!--
-----------------------------------------------------
    Turning the feature area into cards with the the tags below.
-----------------------------------------------------
-->

{% assign featured_projects = site.projects | where: "featured", true %}

<div class="project-grid">
{% for project in featured_projects %}
  <div class="project-card">
    {% if project.image %}
      <img src="{{ project.image }}" alt="{{ project.title }} screenshot">
    {% endif %}
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