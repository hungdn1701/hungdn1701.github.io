---
layout: page
title: Service-Oriented Software Development
order: 2
course_code: INT1448
credits: 3
semester: "Semester II, 2025–2026"
lang: en
year: 2026
archived: false
---

## Course Information

| Code    | Credits | Lecture | Seminar | Semester      |
| ------- | ------- | ------- | ------- | ------------- |
| INT1448 | 3       | 36 hrs  | 18 hrs  | II, 2025–2026 |

**Instructor:** Hung Dang — hungdn@ptit.edu.vn

## Learning Objectives

Upon completion of this course, students will be able to:

1. Analyze and design service-oriented software systems
2. Develop applications using Microservices architecture
3. Deploy and operate systems with CI/CD pipelines

## Course Schedule

### Part 1: Theory (Weeks 1–4)

**Reference**: [Microservices Patterns: With Examples in Java](https://www.manning.com/books/microservices-patterns) by C. Richardson (see **References** section below).

| Week | Topic                              |
| ---- | ---------------------------------- |
| 1    | Course Introduction                |
| 2    | Service-Oriented Architecture      |
| 3    | Service Analysis and Decomposition |
| 4    | API Design and Communication       |

### Part 2: Seminar (Weeks 5–9)

**References**: [Microservices Patterns: With Examples in Java](/assets/materials/service-oriented-development-en/resources/2.%20Microservices%20Patterns%20With%20examples%20in%20Java.pdf) and [Microservices: Up and Running](/assets/materials/service-oriented-development-en/resources/3.%20Microservices-Up-and-Running_complete.pdf)

**Seminar Topics & Resources**: [GitHub Gist - Seminar Materials](#) *(Link to be provided)*

#### Seminar Schedule (5 weeks)

| Week | Topic                          | Coverage                                                                       | Book References           |
| ---- | ------------------------------ | ------------------------------------------------------------------------------ | ------------------------- |
| 5    | Service Gateway & Discovery    | API Gateway, Service Discovery, service registry (Consul/Eureka), edge routing | Richardson Ch3, Mitra Ch4 |
| 6    | Communication Styles           | Sync (REST/gRPC), Async messaging, idempotency, at-least-once delivery         | Richardson Ch3, Mitra Ch3 |
| 7    | Transactional Messaging & Saga | Transactional Outbox, Saga (choreography/orchestration), eventual consistency  | Richardson Ch5, Mitra Ch6 |
| 8    | Circuit Breaker & Reliability  | Circuit Breaker, Retry, Timeout, Bulkhead, fallback patterns                   | Richardson Ch4, Mitra Ch7 |
| 9    | Observability & Tracing        | Logs, metrics (Prometheus), distributed tracing (Jaeger), health checks        | Richardson Ch6, Mitra Ch6 |

#### Preparation Guidance

**Pre-reading (required)**
- Follow the “Book References” column: read the main chapter + 1–2 related patterns.

**Presentation structure (15 minutes per group)**
1. **Concept** (5 min): What is the pattern? When to use it?
2. **Real-world** (5 min): Case study + 1 paper/blog (2025–2026)
3. **Use Cases & Examples** (3 min): Use cases + illustrative examples (optional code demo)
4. **Q&A** (2 min)

### Part 3: Project (Weeks 10–16)

| Week  | Activity                | Notes              |
| ----- | ----------------------- | ------------------ |
| 10    | Project Kickoff         | Max 3 members/team |
| 11–12 | Development & Review 1  |                    |
| 13–14 | Development & Review 2  |                    |
| 15    | Review 3 & Finalization |                    |
| 16    | Project Defense         |

**Project Collaboration**: [GitHub Classroom](#) *(Link to be provided)*

## Materials

**Pending updates**: Seminar gist link, GitHub Classroom link, seminar slides (Weeks 5–9), project resources (Weeks 10–16).

### Part 1: Theory Materials (Weeks 1–4)

| Week | Topic                              | Slides                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| ---- | ---------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1    | Course Introduction                | [Roadmap - Backend](/assets/materials/service-oriented-development-en/slides/0.%20Road%20map%20backend.pdf)<br>[Roadmap - DevOps](/assets/materials/service-oriented-development-en/slides/0.%20Road%20map%20devops.pdf)<br>[Notes](https://gist.github.com/hungdn1701/fe528b27f155c284e11ab7a4dd322029)                                                                                                                                                                                                                                                                                                                                                                   |
| 2    | Service-Oriented Architecture      | [Introduction](/assets/materials/service-oriented-development-en/slides/0.%20Introduction.pdf)<br>[Chapter 3](/assets/materials/service-oriented-development-en/slides/Chapter%203%20Understanding%20Service-Orientation%20-%20En.pdf)                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| 3    | Service Analysis and Decomposition | [Chapter 4](/assets/materials/service-oriented-development-en/slides/Chapter%204%20Understanding%20Service-Orientation-Architecture%20-%20En.pdf)<br>[Chapter 5](/assets/materials/service-oriented-development-en/slides/Chapter%205%20Understanding%20Layer%20with%20Service%20and%20Microservice%20-%20En.pdf)<br>[Chapter 6](/assets/materials/service-oriented-development-en/slides/Chapter%206%20Analysis%20and%20Modeling%20with%20Web%20Services%20and%20Microservices%20-%20En.pdf)<br>[Chapter 7](/assets/materials/service-oriented-development-en/slides/Chapter%207%20Analysis%20and%20Modeling%20with%20Rest%20Services%20and%20Microservices%20-%20En.pdf) |
| 4    | API Design and Communication       | [Chapter 8](/assets/materials/service-oriented-development-en/slides/Chapter%208%20Service%20API%20and%20Contract%20Design%20with%20WS%20-%20En.pdf)<br>[Chapter 9](/assets/materials/service-oriented-development-en/slides/Chapter%209%20Service%20API%20and%20Contract%20Design%20with%20RS%20and%20Microservice%20-%20En.pdf)                                                                                                                                                                                                                                                                                                                                          |

**How to add multiple slides per week**: Separate with `<br>` in the same cell:
```markdown
[Slides A](/path/to/week-01-a.pdf)<br>[Slides B](/path/to/week-01-b.pdf)
```

### Part 2: Seminar Materials (Weeks 5–9)

| Week | Research Topic                 | Slides                                                                         |
| ---- | ------------------------------ | ------------------------------------------------------------------------------ |
| 5    | Service Gateway & Discovery    | [Slides](/assets/materials/service-oriented-development-en/slides/week-05.pdf) |
| 6    | Communication Styles           | [Slides](/assets/materials/service-oriented-development-en/slides/week-06.pdf) |
| 7    | Transactional Messaging & Saga | [Slides](/assets/materials/service-oriented-development-en/slides/week-07.pdf) |
| 8    | Circuit Breaker & Reliability  | [Slides](/assets/materials/service-oriented-development-en/slides/week-08.pdf) |
| 9    | Observability & Tracing        | [Slides](/assets/materials/service-oriented-development-en/slides/week-09.pdf) |

### Part 3: Project Materials (Weeks 10–16)

| Week  | Activity                | Resources                                                                            |
| ----- | ----------------------- | ------------------------------------------------------------------------------------ |
| 10    | Project Kickoff         | [Resources](/assets/materials/service-oriented-development-en/resources/week-10.zip) |
| 11–12 | Development & Review 1  | [Resources](/assets/materials/service-oriented-development-en/resources/week-11.zip) |
| 13–14 | Development & Review 2  | [Resources](/assets/materials/service-oriented-development-en/resources/week-13.zip) |
| 15    | Review 3 & Finalization | [Resources](/assets/materials/service-oriented-development-en/resources/week-15.zip) |
| 16    | Project Defense         | [Resources](/assets/materials/service-oriented-development-en/resources/week-16.zip) |

## Assessment

| Component  | Weight | Description                                   |
| ---------- | ------ | --------------------------------------------- |
| Attendance | 10%    | Weekly check-in                               |
| Quizzes    | 20%    | MCQ + Seminar presentation                    |
| Project    | 70%    | Group report (40%) + Individual defense (30%) |

## References

**Part 1: Theory**

1. [Material 1](/assets/materials/service-oriented-development-en/resources/1.%20Service-Oriented%20Architecture%20Analysis%20and%20Design%20for%20Services%20and%20Microservices%20-%202nd%20Edition.pdf) — Erl, T. (2016). *Service-Oriented Architecture: Analysis & Design for Services and Microservices* (2nd ed.).

**Part 2: Seminar**

2. [Material 2](/assets/materials/service-oriented-development-en/resources/2.%20Microservices%20Patterns%20With%20examples%20in%20Java.pdf) — Richardson, C. (2018). *Microservices Patterns: With Examples in Java*.
3. [Material 3](/assets/materials/service-oriented-development-en/resources/3.%20Microservices-Up-and-Running_complete.pdf) — Mitra, R., & Nadareishvili, I. (2020). *Microservices: Up and Running*.

## Concurrent Courses and Career Orientation

| Course                              | Position                  |
| ----------------------------------- | ------------------------- |
| Requirements Analysis               | Business Analyst          |
| Service-Oriented Development        | Backend / DevOps Engineer |
| Software Quality Assurance          | QA/QC Engineer            |
| Software Architecture & Development | System Architect          |
