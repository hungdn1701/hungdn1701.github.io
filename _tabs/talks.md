---
layout: page
icon: fas fa-microphone-alt
order: 4
---

## Talks & Presentations

Technical talks and presentations on microservices, system design, and software architecture.

{% if site.talks %}
  {% assign sorted_talks = site.talks | sort: 'date' | reverse %}
  {% for talk in sorted_talks %}
<div class="talk-item" style="margin-bottom: 2rem; padding-bottom: 1.5rem; border-bottom: 1px solid var(--border-color);">
  <h3>
    {{ talk.title }}
  </h3>
  
  {% if talk.event %}
  <p style="font-size: 1em; color: var(--text-muted-color);">
    <i class="fas fa-calendar-day"></i> {{ talk.event }}
  </p>
  {% endif %}
  
  {% if talk.date %}
  <p class="text-muted" style="font-size: 0.9em;">
    <i class="far fa-calendar"></i> {{ talk.date | date: "%B %d, %Y" }}
    {% if talk.location %}
      <span style="margin-left: 1rem;">
        <i class="fas fa-map-marker-alt"></i> {{ talk.location }}
      </span>
    {% endif %}
  </p>
  {% endif %}
  
  {% if talk.description %}
  <p>{{ talk.description }}</p>
  {% endif %}
  
  {% if talk.slides_url or talk.video_url %}
  <p>
    {% if talk.slides_url %}
      <a href="{{ talk.slides_url }}" target="_blank">
        <i class="fas fa-file-powerpoint"></i> Slides
      </a>
    {% endif %}
    {% if talk.video_url %}
      <a href="{{ talk.video_url }}" target="_blank" style="margin-left: 1rem;">
        <i class="fas fa-video"></i> Video
      </a>
    {% endif %}
  </p>
  {% endif %}
</div>
  {% endfor %}
{% else %}
  <p class="text-muted"><em>Talks information coming soon...</em></p>
{% endif %}
