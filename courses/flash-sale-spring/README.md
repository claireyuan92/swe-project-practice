# Course 3 — Flash-Sale (Seckill) System in Spring

Build an e-commerce flash-sale system that takes a 10x traffic spike without
overselling a single item. The core techniques: Redis stock pre-deduction with
atomic Lua scripts, distributed locks, message-queue async ordering, and
rate limiting.

## Tech stack

Java · Spring Boot · Redis (Redisson) · RabbitMQ / Kafka · MySQL / PostgreSQL

## What you build

A production-style seckill system: flash-sale gate, atomic stock deduction,
one-order-per-user, async order confirmation via queue, and outbox/Saga for
reliability — load-tested toward 100k QPS.

## Videos

1. **Shopping Website System Design Masterclass | Spring Boot Production Architecture (Saga, Outbox)** (~1 hr, en)
https://www.youtube.com/watch?v=G4QiwJztW7c
Spring Boot production architecture for a shop at 10k req/s normally and 100k during flash sales; "Inventory and Flash Sales" chapter on atomic reservations and a Redis flash-sale gate to never oversell, plus token-bucket rate limiting, idempotency, outbox and Saga.
2. **Shopify's Architecture to Handle the World's Biggest Flash Sales** (~52 min, en, InfoQ)
https://www.youtube.com/watch?v=MV5Kdwzwcag
Shopify's multi-tenant architecture surviving Black Friday flash-sale bursts — queueing, Nginx + Lua page caching, failure prevention (QCon Plus talk).
3. **How Shopify Survives Black Friday: 489 Million Requests a Minute** (~19 min, en, The Machine Room)
https://www.youtube.com/watch?v=eHTt7Qrqq3g
Step-by-step rebuild of Shopify's flash-sale handling — sharding, pods, edge leaky-bucket throttle in Lua on nginx/OpenResty, queue page, fairness by first-tried time.
4. **Top 10 Scenario Based Spring Boot Microservices Interview Questions** (~21 min, en, The Dip Developer)
https://www.youtube.com/watch?v=hMMHBuDtPrM
Senior Spring Boot scenario Q&A; Q06 covers rate limiting for a 1000 rps flash-sale crash with a Redis token bucket via Spring Cloud Gateway, plus Saga/outbox and multi-level caching.
5. **How to Use Redis in Your Spring Boot Project: Step-by-Step Tutorial** (en, Engineering Digest)
https://www.youtube.com/watch?v=2srQ-RiJHps
Hands-on Redis integration in Spring Boot (setup, caching, sessions) — the Redis foundation seckill patterns (stock pre-deduction, distributed locks, Lua) build on.

## Docs, articles & repos

- **** (CSDN, zh)
https://blog.csdn.net/qq_36021478/article/details/156054363
Complete Chinese walkthrough of a seckill system in Spring Boot 2.7 + Redis (Redisson distributed lock) + RabbitMQ + MySQL 8 — architecture, anti-oversell, one-order-per-user, Redis stock pre-deduction, Lua rate limiting, with full code.
- **How to Build a 100k QPS Seckill System with Spring Boot, Redis, and Lua** (BestHub, en)
https://www.besthub.dev/articles/how-to-build-a-100k-qps-seckill-system-with-spring-boot-redis-and-lua-917ccb6ae58a
Production-grade design for a 100k QPS seckill system — qualification-first + async order confirmation, Redis + Lua atomic stock deduction with duplicate-purchase checks, Kafka/RocketMQ async ordering, pre-warming, fault tolerance.
- **high-concurrency-seckill-system** (GitHub — Kazama1996, en)
https://github.com/kazama1996/high-concurrency-seckill-system/blob/HEAD/CLAUDE.md
Production-grade flash-sale system in Spring Boot 3.5.10 / Java 21 with Redis 7 via Redisson (RLock, Bloom filter), atomic Lua stock deduction, Kafka async orders, PostgreSQL, Resilience4j circuit breakers, Outbox pattern; Docker Compose setup included.
