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

## Kế hoạch học tập

### Phần 1 — Lý thuyết (Giảng viên trình bày)

| Tuần | Chủ đề / Hoạt động           | Nội dung                       |
| ---- | ---------------------------- | ------------------------------ |
| 1    | Giới thiệu môn học           | Roadmap, tổng quan môn học     |
| 2    | Kiến trúc hướng dịch vụ      | Khái niệm SOA, nguyên lý       |
| 3    | Phân tích và phân rã dịch vụ | Phân tầng dịch vụ, mô hình hóa |
| 4    | Thiết kế API và giao tiếp    | REST, hợp đồng dịch vụ         |

---

### Phần 2 — Seminar (Sinh viên trình bày)

| Tuần | Chủ đề Seminar                 | Ghi chú                                           |
| ---- | ------------------------------ | ------------------------------------------------- |
| 5    | Service Gateway & Discovery    | API Gateway, Consul/Eureka, edge routing          |
| 6    | Communication Styles           | REST vs gRPC, async messaging, idempotency        |
| 7    | Transactional Messaging & Saga | Outbox pattern, Saga (choreography/orchestration) |
| 8    | Circuit Breaker & Reliability  | Retry, Timeout, Bulkhead, fallback                |
| 9    | Observability & Tracing        | Logs, metrics, distributed tracing                |

---

### Phần 3 — Dự án

| Tuần  | Hoạt động             | Ghi chú                 |
| ----- | --------------------- | ----------------------- |
| 10    | Khởi động dự án       | Chia nhóm (tối đa 3 SV) |
| 11–12 | Phát triển & Review 1 | Phát triển từng phần    |
| 13–14 | Phát triển & Review 2 | Hoàn thiện chức năng    |
| 15    | Review & Hoàn thiện   | Chốt sản phẩm           |
| 16    | Bảo vệ dự án          | Bảo vệ cá nhân          |

## Slide & Học liệu

### Tuần 1 — Giới thiệu môn học
- [Roadmap - Backend](/assets/materials/service-oriented-development-en/slides/0.%20Road%20map%20backend.pdf)
- [Roadmap - DevOps](/assets/materials/service-oriented-development-en/slides/0.%20Road%20map%20devops.pdf)
- [Notes](https://gist.github.com/hungdn1701/fe528b27f155c284e11ab7a4dd322029)

### Tuần 2 — Kiến trúc hướng dịch vụ
- [Introduction](/assets/materials/service-oriented-development-en/slides/0.%20Introduction.pdf)
- [Chapter 3](/assets/materials/service-oriented-development-en/slides/Chapter%203%20Understanding%20Service-Orientation%20-%20En.pdf)

### Tuần 3 — Phân tích và phân rã dịch vụ
- [Chapter 4](/assets/materials/service-oriented-development-en/slides/Chapter%204%20Understanding%20Service-Orientation-Architecture%20-%20En.pdf)
- [Chapter 5](/assets/materials/service-oriented-development-en/slides/Chapter%205%20Understanding%20Layer%20with%20Service%20and%20Microservice%20-%20En.pdf)
- [Chapter 6](/assets/materials/service-oriented-development-en/slides/Chapter%206%20Analysis%20and%20Modeling%20with%20Web%20Services%20and%20Microservices%20-%20En.pdf)
- [Chapter 7](/assets/materials/service-oriented-development-en/slides/Chapter%207%20Analysis%20and%20Modeling%20with%20Rest%20Services%20and%20Microservices%20-%20En.pdf)

### Tuần 4 — Thiết kế API và giao tiếp
- [Chapter 8](/assets/materials/service-oriented-development-en/slides/Chapter%208%20Service%20API%20and%20Contract%20Design%20with%20WS%20-%20En.pdf)
- [Chapter 9](/assets/materials/service-oriented-development-en/slides/Chapter%209%20Service%20API%20and%20Contract%20Design%20with%20RS%20and%20Microservice%20-%20En.pdf)

### Tuần 5 — Service Gateway & Discovery
- *(Slide sẽ cập nhật sau)*

### Tuần 6 — Communication Styles
- *(Slide sẽ cập nhật sau)*

### Tuần 7 — Transactional Messaging & Saga
- *(Slide sẽ cập nhật sau)*

### Tuần 8 — Circuit Breaker & Reliability
- *(Slide sẽ cập nhật sau)*

### Tuần 9 — Observability & Tracing
- *(Slide sẽ cập nhật sau)*


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

## Seminar & Dự án

- **Chủ đề Seminar & Tài liệu**: *(Link sẽ cập nhật sau)*
- **Hợp tác dự án**: *(Link sẽ cập nhật sau)*

