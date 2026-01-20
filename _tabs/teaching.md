---
layout: page
icon: fas fa-chalkboard-teacher
order: 2
---

Faculty member at PTIT since 2016. Teaching systems-oriented, industry-relevant software engineering.

---

## Courses

{% assign sorted_courses = site.teaching | sort: 'order' %}
{% for course in sorted_courses %}
- **[{{ course.title }}]({{ course.url | relative_url }})** — {{ course.credits }} credits {% if course.lang == 'en' %}🇬🇧{% else %}🇻🇳{% endif %}
{% endfor %}

## Other Modules

- Web programming, databases, C systems programming — intensive labs and workshops

## Teaching Approach

- **Project-based** — labs, group projects, case studies
- **Industry-oriented** — design trade-offs, testing, observability
- **Mentoring** — capstone projects and thesis supervision

---

📧 [hungdn@ptit.edu.vn](mailto:hungdn@ptit.edu.vn)
