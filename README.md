# 🚀 8-Week System Design Master Guide (LLD + HLD)
> **Resources Primary Duo:** 
> - **AlgoMaster** (Architectural structure, diagrams, class design templates, and step-by-step text guides)
> - **Gaurav Sen / `@gkcs`** (First-principles depth, mathematical bounds, concurrency, and trade-off justification)

---

## 🛠️ The 3-Step Execution Blueprint
1. **Blueprint (AlgoMaster / 30% time):** Read the target topic/module on AlgoMaster or `awesome-low-level-design`. Learn class diagrams, definitions, and component wiring.
2. **First-Principles Deep Dive (Gaurav Sen / 40% time):** Watch Gaurav Sen's corresponding deep dive. Focus on *why* choices are made, handling edge cases, locking mechanisms, and mathematical bounds.
3. **Active Practice (30% time):** Spend 45 minutes coding the class structures or drawing the system architecture out loud without checking the solution.

---

## 🗓️ Phase 1: Low-Level Design (LLD) & Machine Coding (Weeks 1–2)

### Week 1: OOP, SOLID, & Core Design Patterns

#### Days 1–3: Object-Oriented Programming & SOLID Principles
* **Core Focus:** Class relationships (Association vs Aggregation vs Composition), Abstraction, Encapsulation, Polymorphism.
* **SOLID Breakdown:** Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, Dependency Inversion.
* 📚 **AlgoMaster:** [SOLID Principles Guide](https://algomaster.io/learn/lld/solid-principles)
* 📺 **Gaurav Sen:** [Object-Oriented Design & SOLID Concepts](https://www.youtube.com/watch?v=1b_p3GvOInU)

#### Days 4–7: Core Design Patterns
* **Creational:** Factory Method, Abstract Factory, Singleton, Builder.
* **Structural:** Adapter, Decorator, Facade, Proxy.
* **Behavioral:** Strategy, Observer, Command, State, Chain of Responsibility.
* 📚 **AlgoMaster:** [LLD Design Patterns Catalog](https://algomaster.io/learn/lld)
* 📺 **Gaurav Sen:** [Design Patterns Playlist](https://www.youtube.com/watch?v=v9ejT8FO-7I)

---

### Week 2: Machine Coding & Multi-Threading Practice

#### Days 8–10: State Management & Game Loops
* **Design Tic-Tac-Toe & Snake & Ladder:**
  * *Focus:* Entity modeling, game loop execution, win-condition evaluation.
  * 📚 **AlgoMaster:** [Machine Coding Problems](https://algomaster.io/learn/lld)

#### Days 11–14: Concurrency & Lock Management
* **Design an In-Memory LRU Cache (with TTL):**
  * *Focus:* Doubly Linked List + HashMap, thread-safe access, mutexes, eviction strategies.
  * 📺 **Gaurav Sen:** [LRU Cache Deep Dive](https://www.youtube.com/watch?v=7ABLItLLEVc)
* **Design an Elevator System:**
  * *Focus:* Scheduling algorithms (LOOK/SCAN), state transitions, thread dispatchers.
  * 📺 **Gaurav Sen:** [Elevator System Design](https://www.youtube.com/watch?v=siqiJAJWUUg)
* **Design Parking Lot / BookMyShow:**
  * *Focus:* Concurrent seat/spot allocation, optimistic vs pessimistic locking.
  * 📚 **AlgoMaster:** [Parking Lot & Movie Booking System](https://algomaster.io/learn/lld)

---

## 🗓️ Phase 2: High-Level Design (HLD) Building Blocks (Weeks 3–4)

### Week 3: Networking, Load Balancing & Caching

#### Days 15–17: Networking & Load Balancing
* **Protocols:** TCP vs UDP, HTTP/1.1 vs HTTP/2 vs HTTP/3, WebSockets, gRPC.
* **Load Balancers:** L4 vs L7 Load Balancing, Reverse Proxies (Nginx/HAProxy), Round Robin, Least Connections.
* 📚 **AlgoMaster:** [System Design Fundamentals](https://algomaster.io/learn/system-design)
* 📺 **Gaurav Sen:** [Load Balancers & Reverse Proxies](https://www.youtube.com/watch?v=K0Ta65OqQkY)

#### Days 18–21: Caching Mechanisms & Edge Protection
* **Caching Patterns:** Cache-Aside, Read-Through, Write-Through, Write-Behind.
* **System Failures:** Cache Stampede, Cache Penetration, Cache Avalanche.
* 📚 **AlgoMaster:** [Caching Deep Dive](https://algomaster.io/learn/system-design)
* 📺 **Gaurav Sen:** [Cache Eviction Policies & Caching Strategies](https://www.youtube.com/watch?v=xI_D4S8_0sU)

---

### Week 4: Database Architectures, Sharding & Rate Limiting

#### Days 22–25: Database Scaling & Distributed Data
* **SQL vs NoSQL:** Relational vs Key-Value (Redis/DynamoDB) vs Wide-Column (Cassandra).
* **Scaling Techniques:** Read Replicas, Horizontal Sharding, Connection Pooling, Denormalization.
* **Core Rules:** CAP Theorem, PACELC Theorem, BASE vs ACID.
* 📚 **AlgoMaster:** [Databases & Database Scaling](https://algomaster.io/learn/system-design)
* 📺 **Gaurav Sen:** [Database Sharding vs Partitioning](https://www.youtube.com/watch?v=5faMjKuB9bc)

#### Days 26–28: API Gateways & Security
* **Rate Limiting:** Token Bucket, Leaky Bucket, Fixed Window, Sliding Window Counter algorithms.
* **Security:** JWT, OAuth 2.0, SSL Termination, API Gateway routing.
* 📚 **AlgoMaster:** [Rate Limiting Modules](https://algomaster.io/learn/system-design)
* 📺 **Gaurav Sen:** [Rate Limiting Algorithms & Architecture](https://www.youtube.com/watch?v=CRGPbCbRfZ8)

---

## 🗓️ Phase 3: Advanced Distributed Systems & Scale (Weeks 5–6)

### Week 5: Asynchronous Messaging & Consensus

#### Days 29–32: Message Queues & Event-Driven Systems
* **Broker Mechanics:** Message Queues vs Pub/Sub (Apache Kafka, RabbitMQ, AWS SQS).
* **Patterns:** Change Data Capture (CDC), Outbox Pattern, Dead Letter Queues (DLQ), At-least-once vs Exactly-once processing.
* 📚 **AlgoMaster:** [Communication Patterns](https://algomaster.io/learn/system-design)
* 📺 **Gaurav Sen:** [Message Queues & Pub/Sub Explained](https://www.youtube.com/watch?v=oUJbuF15B48)

#### Days 33–35: Distributed System Mechanics
* **Consistent Hashing:** Ring topology, Virtual Nodes (resolving key hotspots).
* **Consensus & Coordination:** Raft Algorithm, Leader Election, Distributed Locks (Redlock), Zookeeper.
* **Distributed Transactions:** Two-Phase Commit (2PC), SAGA Pattern.
* 📚 **AlgoMaster:** [Distributed System Fundamentals](https://algomaster.io/learn/system-design)
* 📺 **Gaurav Sen:** [Consistent Hashing](https://www.youtube.com/watch?v=zaRkONvyl8s) & [Distributed Locks](https://www.youtube.com/watch?v=5Uytf91xOqQ)

---

### Week 6: High-Scale Data Structures & Spatial Indexing

#### Days 36–42: Specialized Algorithms
* **Bloom Filters:** Probabilistic set membership, false positive trade-offs.
* **Geohash & QuadTrees:** Spatial indexing for proximity/location queries.
* **HyperLogLog & Count-Min Sketch:** Cardinality estimation and frequency tracking.
* 📚 **AlgoMaster:** [Data Structures for Scale](https://algomaster.io/learn/system-design)
* 📺 **Gaurav Sen:** [Geohashing & QuadTrees](https://www.youtube.com/watch?v=M4lR_Va97cQ) & [Bloom Filters](https://www.youtube.com/watch?v=V3pzxngeLqw)

---

## 🗓️ Phase 4: End-to-End System Case Studies (Weeks 7–8)

For each case study, follow this **Interview Checklist**:
1. Clarify Requirements (Functional & Non-Functional).
2. Estimate Capacity (Back-of-the-envelope: QPS, Bandwidth, Storage).
3. Define API Contracts & Data Schema.
4. Draw High-Level Architecture Flow.
5. Deep dive into Single Points of Failure (SPOF) & Bottlenecks.

---

### Master Case Studies Matrix

| System Case Study | Primary Focus & Challenges | Resource Link |
|---|---|---|
| **1. URL Shortener (TinyURL)** | Base62 encoding, Hash collisions, High-read caching | 📚 [AlgoMaster System Case Studies](https://algomaster.io/learn/system-design) |
| **2. Distributed Rate Limiter** | Token Bucket algorithm, Redis atomic counters, Sliding Window | 📺 [Gaurav Sen – Rate Limiter](https://www.youtube.com/watch?v=CRGPbCbRfZ8) |
| **3. Notification System** | Multi-channel dispatch, Idempotency keys, Priority Queues | 📚 [AlgoMaster System Case Studies](https://algomaster.io/learn/system-design) |
| **4. Chat Service (WhatsApp)** | WebSockets, Connection Managers, Cassandra message store | 📺 [Gaurav Sen – Design WhatsApp](https://www.youtube.com/watch?v=vvhC64hQZMk) |
| **5. Social Media Feed (Twitter)** | Fanout-on-write vs Fanout-on-read, Redis timeline caches | 📺 [Gaurav Sen – Design News Feed](https://www.youtube.com/watch?v=QmX2NPkJTKg) |
| **6. Video Streaming (YouTube/Netflix)** | Chunking pipelines, CDNs, Adaptive Bitrate Streaming (HLS) | 📺 [Gaurav Sen – Design Netflix](https://www.youtube.com/watch?v=psQzyFfsUGU) |
| **7. Ride-Hailing App (Uber)** | Spatial indexing (Geohash/QuadTrees), Matchmaking drivers | 📺 [Gaurav Sen – Design Uber](https://www.youtube.com/watch?v=J3DY3Te3A_A) |
| **8. Distributed File System (Google Drive)** | Chunking, Metadata DB sync, Block storage deduplication | 📚 [AlgoMaster System Case Studies](https://algomaster.io/learn/system-design) |
| **9. Location Matching (Tinder)** | Bidirectional matching, Radius spatial queries | 📺 [Gaurav Sen – Design Tinder](https://www.youtube.com/watch?v=tndzLznQq4E) |
| **10. E-Commerce Checkout (Amazon)** | Inventory reservation, SAGA pattern, Payment locking | 📺 [Gaurav Sen – Design E-Commerce](https://www.youtube.com/watch?v=e_p33InBimU) |
