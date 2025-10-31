---
layout: page
icon: fas fa-folder-open
order: 2
---

## My Projects

Here are some of my notable projects in backend development, microservices, and system architecture.

{% if site.projects %}
  {% assign sorted_projects = site.projects | sort: 'order' %}
  {% for project in sorted_projects %}
<div class="project-item" style="margin-bottom: 2rem; padding-bottom: 1.5rem; border-bottom: 1px solid var(--border-color);">
  <h3>
    {{ project.title }}
  </h3>
  
  {% if project.date %}
  <p class="text-muted" style="font-size: 0.9em;">
    <i class="far fa-calendar"></i> {{ project.date | date: "%B %Y" }}
  </p>
  {% endif %}
  
  {% if project.description %}
  <p>{{ project.description }}</p>
  {% endif %}
  
  {% if project.tech_stack %}
  <p style="font-size: 0.9em;">
    <strong>Tech Stack:</strong> {{ project.tech_stack }}
  </p>
  {% endif %}
  
  {% if project.github_url or project.demo_url %}
  <p>
    {% if project.github_url %}
      <a href="{{ project.github_url }}" target="_blank">
        <i class="fab fa-github"></i> GitHub
      </a>
    {% endif %}
    {% if project.demo_url %}
      <a href="{{ project.demo_url }}" target="_blank" style="margin-left: 1rem;">
        <i class="fas fa-external-link-alt"></i> Demo
      </a>
    {% endif %}
  </p>
  {% endif %}
</div>
  {% endfor %}
{% else %}
  <p class="text-muted"><em>Projects coming soon...</em></p>
{% endif %}
