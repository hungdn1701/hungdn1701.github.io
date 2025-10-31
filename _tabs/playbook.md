---
layout: page
icon: fas fa-book-open
order: 6
---

## Technical Playbook

Best practices, guidelines, and technical notes on backend development, microservices, and system design.

{% if site.playbook %}
  {% assign sorted_playbook = site.playbook | sort: 'order' %}
  {% for item in sorted_playbook %}
<div class="playbook-item" style="margin-bottom: 2rem; padding-bottom: 1.5rem; border-bottom: 1px solid var(--border-color);">
  <h3>
    {% if item.url %}
      <a href="{{ item.url | relative_url }}">{{ item.title }}</a>
    {% else %}
      {{ item.title }}
    {% endif %}
  </h3>
  
  {% if item.category %}
  <p style="font-size: 0.9em;">
    <span class="badge badge-primary" style="background-color: var(--link-color); color: white; padding: 0.25rem 0.5rem; border-radius: 0.25rem;">
      {{ item.category }}
    </span>
  </p>
  {% endif %}
  
  {% if item.description %}
  <p>{{ item.description }}</p>
  {% endif %}
  
  {% if item.tags %}
  <p style="font-size: 0.9em; color: var(--text-muted-color);">
    <i class="fas fa-tags"></i> {{ item.tags | join: ", " }}
  </p>
  {% endif %}
  
  {% if item.updated %}
  <p class="text-muted" style="font-size: 0.85em;">
    <i class="far fa-clock"></i> Last updated: {{ item.updated | date: "%B %d, %Y" }}
  </p>
  {% endif %}
</div>
  {% endfor %}
{% else %}
  <p class="text-muted"><em>Playbook content coming soon...</em></p>
{% endif %}
