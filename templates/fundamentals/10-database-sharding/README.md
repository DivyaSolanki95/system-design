# Database Sharding

## What is Sharding?

Sharding splits a large database into multiple smaller databases called shards.

Each shard stores only part of the data.

---

## Why Sharding?

As data grows, a single database cannot efficiently store or process everything.

---

## Example

Shard 1

Users A–F

Shard 2

Users G–M

Shard 3

Users N–Z

---

## Advantages

- Horizontal Scaling
- Better Performance
- Reduced Database Load

---

## Challenges

- Complex Queries
- Rebalancing
- Cross-Shard Transactions

---

## Spring Boot Connection

Large-scale applications distribute users across multiple databases.

---

## Interview Questions

1. What is sharding?
2. Difference between sharding and replication?
3. Why do large companies shard databases?