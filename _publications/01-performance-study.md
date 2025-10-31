---
title: "Performance Analysis of Message Queue Systems in Microservices Architecture"
authors: "Hung Dang, et al."
venue: "International Conference on Software Engineering (ICSE)"
date: 2024-03-20
abstract: "A comprehensive performance study comparing Kafka, RabbitMQ, and NATS in microservices environments under various load patterns."
paper_url: ""
doi: ""
code_url: ""
---

## Abstract

Message queue systems play a crucial role in microservices architecture, enabling asynchronous communication and decoupling between services. This paper presents a comprehensive performance evaluation of three popular message queue systems: Apache Kafka, RabbitMQ, and NATS.

## Key Findings

- **Throughput**: Kafka demonstrated superior throughput for high-volume scenarios
- **Latency**: NATS showed lowest latency for real-time messaging
- **Resource Usage**: RabbitMQ offered the best balance of features and resource efficiency

## Methodology

- Load testing with varying message sizes (1KB - 10MB)
- Multiple producer/consumer configurations
- Network latency simulation
- Failure scenario testing

## Conclusions

The choice of message queue system should be driven by specific use case requirements rather than popularity. Our findings provide practical guidance for architects selecting messaging infrastructure.
