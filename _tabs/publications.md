---
layout: page
icon: fas fa-book
order: 5
---

## Publications & Research

Publications are listed by year (most recent first) and labeled as journal or conference.

{% assign pubs = site.publications | sort: 'date' | reverse %}

{%- comment -%} International journals {%- endcomment -%}
### International journals
{% assign internationals = pubs | where: "category", "journal-international" %}
{% if internationals and internationals != empty %}
  {% assign last_year = "" %}
  {% for pub in internationals %}
    {% assign py = pub.date | date: "%Y" %}
    {% if py != last_year %}
      <h4 style="margin-top:1.25rem">{{ py }}</h4>
      {% assign last_year = py %}
    {% endif %}
    <p style="margin:0">
      {% if pub.authors %}{{ pub.authors }}. {% endif %}
      <strong>{{ pub.title }}</strong>.
      {% if pub.venue %} {{ pub.venue }}{% endif %}
      {% if pub.pages %}, pp. {{ pub.pages }}{% endif %}
      {% if pub.date %}, {{ pub.date | date: "%Y" }}{% endif %}.
      {% if pub.doi and pub.doi != '' %}
        <a href="https://doi.org/{{ pub.doi }}" target="_blank">DOI</a>
      {% endif %}
      {% if pub.paper_url and pub.paper_url != '' %}
        <a href="{{ pub.paper_url }}" target="_blank" style="margin-left:0.5rem">Paper</a>
      {% endif %}
    </p>
  {% endfor %}
{% else %}
  <p class="text-muted"><em>No international journal entries yet.</em></p>
{% endif %}

{%- comment -%} National journals {%- endcomment -%}
### National / Local journals
{% assign nationals = pubs | where: "category", "journal-national" %}
{% if nationals and nationals != empty %}
  {% assign last_year = "" %}
  {% for pub in nationals %}
    {% assign py = pub.date | date: "%Y" %}
    {% if py != last_year %}
      <h4 style="margin-top:1.25rem">{{ py }}</h4>
      {% assign last_year = py %}
    {% endif %}
    <p style="margin:0">
      {% if pub.authors %}{{ pub.authors }}. {% endif %}
      <strong>{{ pub.title }}</strong>.
      {% if pub.venue %} {{ pub.venue }}{% endif %}
      {% if pub.pages %}, pp. {{ pub.pages }}{% endif %}
      {% if pub.date %}, {{ pub.date | date: "%Y" }}{% endif %}.
      {% if pub.doi and pub.doi != '' %}
        <a href="https://doi.org/{{ pub.doi }}" target="_blank">DOI</a>
      {% endif %}
      {% if pub.paper_url and pub.paper_url != '' %}
        <a href="{{ pub.paper_url }}" target="_blank" style="margin-left:0.5rem">Paper</a>
      {% endif %}
    </p>
  {% endfor %}
{% else %}
  <p class="text-muted"><em>No national journal entries yet.</em></p>
{% endif %}

{%- comment -%} Conferences {%- endcomment -%}
### Conference proceedings
{% assign confs = pubs | where: "category", "conference" %}
{% if confs and confs != empty %}
  {% assign last_year = "" %}
  {% for pub in confs %}
    {% assign py = pub.date | date: "%Y" %}
    {% if py != last_year %}
      <h4 style="margin-top:1.25rem">{{ py }}</h4>
      {% assign last_year = py %}
    {% endif %}
    <p style="margin:0">
      {% if pub.authors %}{{ pub.authors }}. {% endif %}
      <strong>{{ pub.title }}</strong>.
      {% if pub.venue %} {{ pub.venue }}{% endif %}
      {% if pub.pages %}, pp. {{ pub.pages }}{% endif %}
      {% if pub.date %}, {{ pub.date | date: "%Y" }}{% endif %}.
      {% if pub.doi and pub.doi != '' %}
        <a href="https://doi.org/{{ pub.doi }}" target="_blank">DOI</a>
      {% endif %}
      {% if pub.paper_url and pub.paper_url != '' %}
        <a href="{{ pub.paper_url }}" target="_blank" style="margin-left:0.5rem">Paper</a>
      {% endif %}
    </p>
  {% endfor %}
{% else %}
  <p class="text-muted"><em>No conference entries yet.</em></p>
{% endif %}
