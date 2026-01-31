---
layout: page
title: Phát triển phần mềm hướng dịch vụ
order: 1
course_code: INT1448
credits: 3
semester: "Semester II, 2025–2026"
lang: vi
year: 2026
archived: false
---

## Thông tin chung

| Mã học phần | Tín chỉ | Lý thuyết | Thảo luận | Học kỳ        |
| ----------- | ------- | --------- | --------- | ------------- |
| INT1448     | 3       | 36 tiết   | 18 tiết   | II, 2025–2026 |

**Giảng viên:** Đặng Ngọc Hùng — hungdn@ptit.edu.vn

## Mục tiêu

Sau khi hoàn thành môn học, sinh viên có khả năng:

1. Phân tích và thiết kế hệ thống phần mềm hướng dịch vụ
2. Phát triển ứng dụng theo kiến trúc Microservices
3. Triển khai và vận hành hệ thống với CI/CD

## Kế hoạch & Học liệu tổng hợp

| Tuần  | Chủ đề / Hoạt động             | Nội dung / Ghi chú                                                             | Slide / Tài liệu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| ----- | ------------------------------ | ------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1     | Giới thiệu môn học             |                                                                                | [Roadmap - Backend](/assets/materials/service-oriented-development-en/slides/0.%20Road%20map%20backend.pdf)<br>[Roadmap - DevOps](/assets/materials/service-oriented-development-en/slides/0.%20Road%20map%20devops.pdf)<br>[Notes](https://gist.github.com/hungdn1701/fe528b27f155c284e11ab7a4dd322029)                                                                                                                                                                                                                                                                                                                                                                   |
| 2     | Kiến trúc hướng dịch vụ        |                                                                                | [Introduction](/assets/materials/service-oriented-development-en/slides/0.%20Introduction.pdf)<br>[Chapter 3](/assets/materials/service-oriented-development-en/slides/Chapter%203%20Understanding%20Service-Orientation%20-%20En.pdf)                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| 3     | Phân tích và phân rã dịch vụ   |                                                                                | [Chapter 4](/assets/materials/service-oriented-development-en/slides/Chapter%204%20Understanding%20Service-Orientation-Architecture%20-%20En.pdf)<br>[Chapter 5](/assets/materials/service-oriented-development-en/slides/Chapter%205%20Understanding%20Layer%20with%20Service%20and%20Microservice%20-%20En.pdf)<br>[Chapter 6](/assets/materials/service-oriented-development-en/slides/Chapter%206%20Analysis%20and%20Modeling%20with%20Web%20Services%20and%20Microservices%20-%20En.pdf)<br>[Chapter 7](/assets/materials/service-oriented-development-en/slides/Chapter%207%20Analysis%20and%20Modeling%20with%20Rest%20Services%20and%20Microservices%20-%20En.pdf) |
| 4     | Thiết kế API và giao tiếp      |                                                                                | [Chapter 8](/assets/materials/service-oriented-development-en/slides/Chapter%208%20Service%20API%20and%20Contract%20Design%20with%20WS%20-%20En.pdf)<br>[Chapter 9](/assets/materials/service-oriented-development-en/slides/Chapter%209%20Service%20API%20and%20Contract%20Design%20with%20RS%20and%20Microservice%20-%20En.pdf)                                                                                                                                                                                                                                                                                                                                          |
| 5     | Service Gateway & Discovery    | API Gateway, Service Discovery, service registry (Consul/Eureka), edge routing | *(Slide sẽ cập nhật sau)*                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| 6     | Communication Styles           | Sync (REST/gRPC), Async messaging, idempotency, at-least-once delivery         | *(Slide sẽ cập nhật sau)*                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| 7     | Transactional Messaging & Saga | Transactional Outbox, Saga (choreography/orchestration), eventual consistency  | *(Slide sẽ cập nhật sau)*                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| 8     | Circuit Breaker & Reliability  | Circuit Breaker, Retry, Timeout, Bulkhead, fallback patterns                   | *(Slide sẽ cập nhật sau)*                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| 9     | Observability & Tracing        | Logs, metrics (Prometheus), distributed tracing (Jaeger), health checks        | *(Slide sẽ cập nhật sau)*                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| 10    | Khởi động dự án                | Tối đa 3 thành viên/nhóm                                                       | *(Tài liệu dự án sẽ cập nhật sau)*                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| 11–13 | Phát triển & Review            | ~1/3 lớp mỗi tuần                                                              | *(Tài liệu dự án sẽ cập nhật sau)*                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| 14–15 | Hoàn thiện & Bảo vệ            |                                                                                | *(Tài liệu dự án sẽ cập nhật sau)*                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| 16    | Dự phòng                       |                                                                                | *(Tài liệu dự án sẽ cập nhật sau)*                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |

**Tài liệu tham khảo**: [Microservices Patterns: With Examples in Java](/assets/materials/service-oriented-development-en/resources/2.%20Microservices%20Patterns%20With%20examples%20in%20Java.pdf), [Microservices: Up and Running](/assets/materials/service-oriented-development-en/resources/3.%20Microservices-Up-and-Running_complete.pdf)

**Chủ đề Seminar & Tài liệu**: [GitHub Gist - Seminar Materials](#) *(Link sẽ cập nhật sau)*
**Hợp tác dự án**: [GitHub Classroom](#) *(Link sẽ cập nhật sau)*

**Cách thêm nhiều slide trong một tuần**: Tách bằng `<br>` trong cùng một ô:
```markdown
[Slides A](/path/to/week-01-a.pdf)<br>[Slides B](/path/to/week-01-b.pdf)
```

**Hướng dẫn chuẩn bị Seminar**
- Pre-reading: Theo cột “Nội dung / Ghi chú” và tài liệu tham khảo.
- Presentation structure (15p/nhóm): Concept (5), Real-world (5), Use Cases (3), Q&A (2)
## Đánh giá

| Thành phần | Tỷ lệ | Mô tả                                     |
| ---------- | ----- | ----------------------------------------- |
| Chuyên cần | 10%   | Điểm danh hàng tuần                       |
| Kiểm tra   | 20%   | Trắc nghiệm + Báo cáo seminar             |
| Dự án      | 70%   | Báo cáo nhóm (40%) + Bảo vệ cá nhân (30%) |

## Tài liệu tham khảo

**Phần 1: Lý thuyết**

1. [Học liệu 01](/assets/materials/service-oriented-development-en/resources/1.%20Service-Oriented%20Architecture%20Analysis%20and%20Design%20for%20Services%20and%20Microservices%20-%202nd%20Edition.pdf) — Erl, T. (2016). *Service-Oriented Architecture: Analysis & Design for Services and Microservices* (2nd ed.).

**Phần 2: Seminar**

2. [Học liệu 02](/assets/materials/service-oriented-development-en/resources/2.%20Microservices%20Patterns%20With%20examples%20in%20Java.pdf) — Richardson, C. *Microservices Patterns: With Examples in Java*.
3. [Học liệu 03](/assets/materials/service-oriented-development-en/resources/3.%20Microservices-Up-and-Running_complete.pdf) — Mitra, R., & Nadareishvili, I. (2020). *Microservices: Up and Running*.

## Môn học cùng kỳ và Định hướng nghề nghiệp

| Môn học                           | Vị trí                    |
| --------------------------------- | ------------------------- |
| Phân tích yêu cầu                 | Business Analyst          |
| Phát triển phần mềm hướng dịch vụ | Backend / DevOps Engineer |
| Đảm bảo chất lượng phần mềm       | QA/QC Engineer            |
| Kiến trúc và phát triển phần mềm  | System Architect          |
