# Distributed Cache Engine

A high-performance **distributed in-memory cache** built from scratch in **C/C++**, inspired by the internal architecture of Redis. This project focuses on learning and implementing core database and distributed system concepts such as event-driven networking, efficient memory structures, persistence, and clustering.

---

## Repository Description

**Distributed Cache Engine** is an experimental but production-oriented distributed key–value store designed to explore how modern in-memory databases like Redis work internally. The project aims to provide a lightweight, high‑performance caching layer capable of running in distributed environments.

---

# Features

* In-memory key–value storage
* Redis-like command protocol
* High-performance networking (event-driven architecture)
* Efficient memory management
* Persistence (snapshot / append-only log – planned)
* Replication support (planned)
* Clustered distributed nodes (planned)
* Pub/Sub messaging (planned)

---

# Goals

This project is designed to:

1. Understand how Redis works internally
2. Learn systems programming using C/C++
3. Implement networking servers from scratch
4. Explore distributed system design
5. Build a production-style caching engine

---

# Architecture Overview

```
Client
   │
   │  TCP Protocol
   ▼
Network Layer
   │
   ▼
Command Parser
   │
   ▼
Execution Engine
   │
   ▼
In-Memory Storage Engine
   │
   ├── Hash Table
   ├── String
   ├── List
   └── Set
```

Future architecture will include:

* Replication
* Sharding
* Cluster coordination

---

# Project Structure

```
distributed-cache-engine
│
├── src/
│   ├── server/
│   ├── network/
│   ├── protocol/
│   ├── storage/
│   └── cluster/
│
├── include/
├── tests/
├── benchmarks/
├── docs/
└── examples/
```

---

# Build Instructions

### Requirements

* C++17 or newer
* GCC / Clang
* CMake

### Build

```bash
mkdir build
cd build
cmake ..
make
```

---

# Running the Server

```bash
./cache-server
```

Default port:

```
6379
```

---

# Example Commands

```
SET key value
GET key
DEL key
```

---

# Learning Topics Covered

This project explores several core backend and systems concepts:

* Event-driven server architecture
* TCP networking
* Memory management
* Hash table implementation
* Command parsing
* Concurrency and threading
* Distributed systems fundamentals

---

# Roadmap

## Phase 1

* TCP server
* Basic command parser
* Key-value storage

## Phase 2

* Expiration and TTL
* Persistence

## Phase 3

* Replication
* Leader–follower architecture

## Phase 4

* Cluster mode
* Sharding

---

# Inspiration

* Redis
* LevelDB
* RocksDB
* etcd

---

# License

MIT License

---

# Author

Mehedi Hasan

Backend Engineer | Distributed Systems Enthusiast
