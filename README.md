# Java Preparation Guide

A structured collection of Q&As covering core Java, Spring ecosystem, messaging, reactive programming, and SQL — from fundamentals to advanced topics.

---

## Contents

| # | File | Topics Covered |
|---|---|---|
| 1 | [Core Java](1.%20Core-Java.md) | OOP, Collections, Generics, Exception Handling, Concurrency, Memory Model |
| 2 | [Advanced Java](2.%20Advanced-Java.md) | Streams, Lambdas, Optional, Reflection, Design Patterns, JVM Internals |
| 3 | [Spring Boot](3.%20Spring-Boot.md) | Auto-configuration, Starters, Actuator, REST, Profiles, Testing |
| 4 | [Spring Data](4.%20Spring-Data.md) | JPA, Hibernate, Repositories, Projections, Transactions, Redis, Caching |
| 5 | [Apache Kafka](5.%20Apache-Kafka.md) | Producers, Consumers, Topics, Partitions, Consumer Groups, Streams, Error Handling |
| 6 | [Spring Security](6.%20Spring-Security.md) | Authentication, Authorization, JWT, OAuth2, CSRF, Cookies, Security Patterns |
| 7 | [Spring WebFlux](7.%20Spring%20WebFlux.md) | Reactive Streams, Mono/Flux, Back-pressure, WebClient, R2DBC, Testing |
| 8 | [Rabbit MQ](8.%20Rabbit-MQ.md) | Exchanges, Queues, Bindings, Routing, Dead Letter, Spring AMQP |
| 9 | [Apache Kafka](9.%20Active-MQ.md) | Brokers, Destinations, Message Selectors, Spring JMS, Persistence |
| 10 | [SQL](10.%20SQL.md) | DDL/DML/DCL/TCL, Joins, Indexes, Aggregates, Subqueries, Window Functions, Normalization, Transactions, Views, Constraints |
| 11 | [SQL Advanced](11.%20SQL-ADVANCE.md) | CTEs, Recursive Queries, Execution Plans, Partitioning, Materialized Views, Locks, Isolation Levels, Sharding, Anti-Patterns |
| — | [Java Versions](Java-Versions.md) | Key features per Java release (Java 8 → Java 21+) |

---

## Topic Overview

### Core Java
Fundamentals every Java developer must know:
- OOP principles (Encapsulation, Inheritance, Polymorphism, Abstraction)
- Collections Framework (`List`, `Map`, `Set`, `Queue`) and their internal implementations
- Generics, wildcards, and type erasure
- Exception handling — checked vs. unchecked, custom exceptions
- Multithreading and concurrency (`synchronized`, `volatile`, `ExecutorService`, locks)
- Java Memory Model and garbage collection

### Advanced Java
Deeper language features and architectural concepts:
- Functional programming — Streams API, Lambda expressions, method references
- `Optional<T>` for null safety
- Reflection and annotations
- Common design patterns (Singleton, Builder, Factory, Strategy, Observer)
- JVM internals — class loading, bytecode, JIT compilation

### Spring Boot
Building production-ready Spring applications:
- Auto-configuration and `@SpringBootApplication`
- Dependency injection and the Spring IoC container
- REST API development with `@RestController`
- Spring Boot Actuator for health checks and metrics
- Profiles, externalized configuration (`application.yml`)
- Testing with `@SpringBootTest`, `@MockBean`, `MockMvc`

### Spring Data, JPA & Hibernate
Persistent data access:
- JPA specification and `EntityManager`
- Hibernate as a JPA provider — dirty checking, second-level cache, `ddl-auto`
- Entity lifecycle states — Transient, Managed, Detached, Removed
- Relationship mappings — `@OneToMany`, `@ManyToMany`, cascade, fetch strategies
- JPQL, Criteria API, Native Queries
- Spring Data repositories — `JpaRepository`, derived queries, `@Query`
- Projections and DTOs for performance
- `@Transactional` — propagation, isolation, rollback rules
- Redis caching — `RedisCacheManager`, `RedisTemplate`, `@Cacheable`
- N+1 select problem and solutions (`JOIN FETCH`, `@EntityGraph`, `@BatchSize`)

### Apache Kafka
Event streaming and asynchronous messaging:
- Core concepts — brokers, topics, partitions, offsets
- Producers, consumers, and consumer groups
- Message ordering and partition keys
- Kafka Streams for stream processing
- Spring Kafka — `@KafkaListener`, `KafkaTemplate`
- Error handling — dead letter topics, retry, idempotency

### Spring Security
Securing Spring applications:
- Filter chain architecture — `DelegatingFilterProxy`, `SecurityFilterChain`
- Authentication vs Authorization (AuthN vs AuthZ)
- JWT — structure, Access Tokens, Refresh Tokens, rotation
- OAuth2 / OpenID Connect — authorization code flow, resource server
- CSRF protection — Synchronizer Token Pattern, `SameSite` cookies
- Cookie security attributes — `HttpOnly`, `Secure`, `SameSite`
- Authentication patterns — Form Login, HTTP Basic, JWT Bearer, OAuth2, API Key
- Authorization patterns — RBAC, ABAC, PBAC, ReBAC, ACL
- SecurityContext propagation in async and reactive contexts

### Spring WebFlux
Reactive, non-blocking web programming:
- Reactive Streams specification — Publisher, Subscriber, back-pressure
- `Mono<T>` and `Flux<T>` — core reactive types
- Two programming models — annotated controllers and functional endpoints (`RouterFunction`)
- Error handling in reactive pipelines
- `WebClient` — non-blocking HTTP client replacing `RestTemplate`
- Reactive database access — R2DBC, Spring Data Reactive repositories
- Testing with `WebTestClient`

### SQL — Core
Relational database essentials:
- SQL command categories — DDL, DML, DCL, TCL
- `DELETE` vs `TRUNCATE` vs `DROP`
- All JOIN types — INNER, LEFT, RIGHT, FULL OUTER, CROSS, SELF
- `WHERE` vs `HAVING` — filtering rows vs. groups
- Primary Key, Foreign Key, and Unique Key
- Indexes — Clustered, Non-Clustered, Composite, Unique
- Aggregate functions — `COUNT`, `SUM`, `AVG`, `MIN`, `MAX`
- Subqueries — single-row, multi-row, correlated, derived tables
- Window functions — `ROW_NUMBER`, `RANK`, `DENSE_RANK`, `LAG`, `LEAD`
- Normalization — 1NF, 2NF, 3NF with examples
- Transactions and ACID properties
- Views — creation, updatable views, limitations
- `UNION` vs `UNION ALL`
- Stored Procedures vs. Functions
- Constraints — `NOT NULL`, `UNIQUE`, `CHECK`, `DEFAULT`, `FOREIGN KEY`

### SQL — Advanced
Performance, architecture, and production patterns:
- CTEs and Recursive CTEs — hierarchical data traversal (org charts, trees)
- Advanced window functions — frame clauses, rolling averages, `FIRST_VALUE`, `NTH_VALUE`
- Advanced JOINs — LATERAL, Anti-Join, Semi-Join, Non-Equi JOIN
- SQL logical execution order and query optimization
- Reading `EXPLAIN`/`EXPLAIN ANALYZE` output — plan nodes, cost metrics
- Database partitioning — Range, List, Hash partitioning with partition pruning
- Materialized Views — storage, refresh strategies, indexes on views
- Locks and Deadlocks — lock types, deadlock scenarios, `SKIP LOCKED`, prevention
- Isolation levels and concurrency anomalies — dirty reads, phantom reads, lost updates
- OLTP vs OLAP schema design — Star Schema, Fact and Dimension tables
- `GROUPING SETS`, `ROLLUP`, `CUBE` — multi-level aggregations
- Efficient pagination — OFFSET pitfalls, Keyset/Cursor pagination
- Triggers — BEFORE/AFTER/INSTEAD OF, audit log, validation triggers
- Sharding vs Replication — shard key strategies, tradeoffs
- SQL anti-patterns — SELECT *, implicit casts, correlated subqueries, NOT IN with NULLs

### Java Versions
Key language and JVM improvements per release:
- **Java 8** — Lambdas, Streams, `Optional`, default methods, Date/Time API
- **Java 11** — `var` improvements, HTTP Client, `String` utilities
- **Java 14–16** — Records, Sealed Classes (preview), Pattern Matching (`instanceof`)
- **Java 17** — LTS: Records, Sealed Classes (stable), Text Blocks
- **Java 21** — LTS: Virtual Threads (Project Loom), Pattern Matching for `switch`, Sequenced Collections

---

## How to Use

1. Start with **Core Java** to solidify fundamentals.
2. Progress to **Advanced Java** for language-level depth.
3. Study **Spring Boot** as the foundation for the Spring ecosystem.
4. Cover **Spring Data** for persistence knowledge.
5. Study **Spring Security** and **Spring WebFlux** for modern Spring patterns.
6. Review **Apache Kafka** for distributed systems and messaging.
7. Study **SQL** for relational database fundamentals and interview essentials.
8. Study **SQL Advanced** for performance, architecture, and production-grade patterns.
9. Use **Java Versions** as a quick reference for feature timelines.

---

## Study Tips

- Each file follows a **Question → Answer** format; try answering before reading.
- Code examples are provided for every concept — read them carefully.
- Pay attention to **comparison tables** — they are common in interviews.
- Focus on the **"why"** behind each design decision, not just the "what".

---

