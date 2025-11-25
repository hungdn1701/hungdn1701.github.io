---
layout: page
icon: fas fa-chalkboard-teacher
order: 3
---

## Teaching

I've taught since 2013 and officially joined the Faculty of Information Technology at the Posts and Telecommunications Institute of Technology (PTIT) in 2016.

My primary courses (regular/major):

- Service-Oriented Software Development
- Network Programming
- Web Services & Microservices

I also deliver shorter modules and workshops in web programming, databases, and C systems programming.

{% if site.teaching %}
  {% assign sorted_teaching = site.teaching | sort: 'order' %}
  {% for course in sorted_teaching %}
<div class="teaching-item" style="margin-bottom: 2rem; padding-bottom: 1.5rem; border-bottom: 1px solid var(--border-color);">
  <h3>
    {{ course.title }}
  </h3>
  
  {% if course.institution %}
  <p style="font-size: 1em; color: var(--text-muted-color);">
    <i class="fas fa-university"></i> {{ course.institution }}
  </p>
  {% endif %}
  
  {% if course.period %}
  <p class="text-muted" style="font-size: 0.9em;">
    <i class="far fa-calendar"></i> {{ course.period }}
  </p>
  {% endif %}
  
  {% if course.description %}
  <p>{{ course.description }}</p>
  {% endif %}
  
  {% if course.topics %}
  <p style="font-size: 0.9em;">
    <strong>Topics:</strong> {{ course.topics }}
  </p>
  {% endif %}
  
  {% if course.students %}
  <p style="font-size: 0.9em;">
    <strong>Students:</strong> {{ course.students }}
  </p>
  {% endif %}
</div>
  {% endfor %}
{% else %}
  <p class="text-muted"><em>Teaching information coming soon...</em></p>
{% endif %}
