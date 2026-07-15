# Distributed Transactions

## What are Distributed Transactions?

A Distributed Transaction is a transaction that involves multiple independent services or databases.

Unlike a traditional transaction that works within a single database, distributed transactions coordinate changes across multiple systems while trying to maintain data consistency.

---

## Why Do We Need Distributed Transactions?

Imagine an e-commerce application.

When a customer places an order, several services are involved:

- Order Service
- Payment Service
- Inventory Service
- Notification Service

If payment succeeds but inventory fails, the system can become inconsistent.

Distributed transactions help coordinate these operations.

---

## Example

Customer places an order.

↓

Order Service

↓

Payment Service

↓

Inventory Service

↓

Shipping Service

If any critical step fails, the system must recover gracefully.

---

## Challenges

- Network failures
- Partial success
- Rollbacks across services
- High complexity

---

## Common Approaches

### Two-Phase Commit (2PC)

Coordinator asks every service:

"Can you commit?"

If everyone agrees:

Commit.

Otherwise:

Rollback.

Pros

- Strong consistency

Cons

- Slow
- Blocking
- Single coordinator

---

### Saga Pattern

Instead of one large transaction, split the process into multiple local transactions.

If one step fails, execute compensating actions.

Example:

Payment Successful

↓

Inventory Failed

↓

Refund Payment

---

## Spring Boot Connection

Distributed transactions in microservices often use the Saga Pattern with Kafka or RabbitMQ.

---

## Interview Questions

1. What is a Distributed Transaction?
2. Why is 2PC slow?
3. What is the Saga Pattern?
4. Why is Saga preferred in microservices?

---

## Key Takeaways

- Distributed transactions span multiple services.
- 2PC provides strong consistency but has drawbacks.
- Saga is commonly used in modern distributed systems.