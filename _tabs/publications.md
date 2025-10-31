---
layout: page
icon: fas fa-book
order: 5
---

## Publications & Research

Academic papers, articles, and research work in software engineering and system architecture.

{% if site.publications %}
  {% assign sorted_publications = site.publications | sort: 'date' | reverse %}
  {% for pub in sorted_publications %}
<div class="publication-item" style="margin-bottom: 2rem; padding-bottom: 1.5rem; border-bottom: 1px solid var(--border-color);">
  <h3>
    {{ pub.title }}
  </h3>
  
  {% if pub.authors %}
  <p style="font-size: 0.95em; color: var(--text-muted-color);">
    <i class="fas fa-users"></i> {{ pub.authors }}
  </p>
  {% endif %}
  
  {% if pub.venue %}
  <p style="font-size: 0.95em; font-style: italic;">
    {{ pub.venue }}
  </p>
  {% endif %}
  
  {% if pub.date %}
  <p class="text-muted" style="font-size: 0.9em;">
    <i class="far fa-calendar"></i> {{ pub.date | date: "%B %Y" }}
  </p>
  {% endif %}
  
  {% if pub.abstract %}
  <p>{{ pub.abstract }}</p>
  {% endif %}
  
  {% if pub.paper_url or pub.doi or pub.code_url %}
  <p>
    {% if pub.paper_url %}
      <a href="{{ pub.paper_url }}" target="_blank">
        <i class="fas fa-file-pdf"></i> Paper
      </a>
    {% endif %}
    {% if pub.doi %}
      <a href="https://doi.org/{{ pub.doi }}" target="_blank" style="margin-left: 1rem;">
        <i class="fas fa-link"></i> DOI
      </a>
    {% endif %}
    {% if pub.code_url %}
      <a href="{{ pub.code_url }}" target="_blank" style="margin-left: 1rem;">
        <i class="fab fa-github"></i> Code
      </a>
    {% endif %}
  </p>
  {% endif %}
</div>
  {% endfor %}
{% else %}
  <p class="text-muted"><em>Publications coming soon...</em></p>
{% endif %}
