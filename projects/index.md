---
layout: page
title: Projects
permalink: /projects/
---

<div class="project-archive-intro">
  <p>
    This journal captures the systems, studies, and products I iterate on. Each entry includes context, decisions, and the impact
    I'm measuring so collaborators can trace how ideas evolve over time.
  </p>
</div>

<div class="project-archive">
  {% assign sorted_projects = site.projects | sort: 'order' %}
  {% for project in sorted_projects %}
  <article class="project-archive__item">
    {% if project.category %}<span class="project-card__label">{{ project.category }}</span>{% endif %}
    <h2 class="project-archive__title"><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h2>
    <p class="project-archive__summary">{{ project.summary }}</p>
    <ul class="project-archive__meta">
      {% if project.timeline %}<li>{{ project.timeline }}</li>{% endif %}
      {% if project.role %}<li>{{ project.role }}</li>{% endif %}
      {% if project.skills %}<li>{{ project.skills | join: ' · ' }}</li>{% endif %}
    </ul>
  </article>
  {% endfor %}
</div>
