---
layout: page
icon: fas fa-chalkboard-teacher
order: 2
---

## Semester II, 2025–2026

{% assign current_courses = site.teaching | where: "archived", false | sort: 'order' %}
{% for course in current_courses %}
- [{{ course.title }}]({{ course.url | relative_url }}) — {{ course.credits }} credits {% if course.lang == 'en' %}🇬🇧{% else %}🇻🇳{% endif %}
{% endfor %}

## Courses

| Course                       | Year | Topics                             |
| ---------------------------- | ---- | ---------------------------------- |
| C Programming                | 1    | Fundamentals, pointers, memory     |
| OOP                          | 2    | Java/C#, design principles         |
| Web Programming              | 3    | MVC, frontend, backend             |
| Network Programming          | 3    | Sockets, protocols, multithreading |
| Service-Oriented Development | 4    | Microservices, patterns, DevOps    |

## Archive

<details>
<summary>Previous semesters</summary>

**Semester I, 2025–2026**
- Network Programming 🇻🇳

{% assign archived_courses = site.teaching | where: "archived", true | sort: 'year' | reverse %}
{% for course in archived_courses %}
- {{ course.semester }} — [{{ course.title }}]({{ course.url | relative_url }})
{% endfor %}

</details>
