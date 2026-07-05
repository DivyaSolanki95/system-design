# Database Replication

## What is Replication?

Replication is the process of copying data from one database server to one or more replica servers.

---

## Why Replication?

- High Availability
- Fault Tolerance
- Read Scalability

---

## Types

### Primary-Replica

Writes go to the Primary.

Reads can come from Replicas.

---

## Advantages

- Faster reads
- Backup
- Disaster Recovery

---

## Disadvantages

- Replication lag
- More infrastructure

---

## Spring Boot Connection

Applications often read from replicas and write to the primary database.

---

## Interview Questions

1. What is replication?
2. Why use replicas?
3. What is replication lag?