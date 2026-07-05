# Consistent Hashing

## What is Consistent Hashing?

Consistent Hashing is a technique used to distribute data across multiple servers while minimizing data movement when servers are added or removed.

---

## Why Do We Need It?

Without consistent hashing, adding one server may require redistributing almost all data.

With consistent hashing, only a small portion of data moves.

---

## Where is it Used?

- Redis Cluster
- Cassandra
- Distributed Cache
- CDN

---

## Advantages

- Better Scalability
- Minimal Data Movement
- Load Distribution

---

## Spring Boot Connection

Applications using Redis clusters benefit from consistent hashing.

---

## Interview Questions

1. Why consistent hashing?
2. Where is it used?
3. Why not use modulo hashing?