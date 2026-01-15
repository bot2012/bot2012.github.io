---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Home
---




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

<h2>Short Blog Posts</h2>

<ul class="post-list">
  {% for post in site.posts limit:4 %}
    <li>
      <h3>
        <a href="{{ post.url }}">{{ post.title }}</a>
      </h3>
      <p>{{ post.excerpt }}</p>
      <small>{{ post.date | date: "%B %d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>

<h2> Featured Projects </h2>

{% assign featured_projects = site.projects | where: "featured", true | sort: "order" %}

<div class="project-grid">
{% for project in featured_projects limit:4 %}
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