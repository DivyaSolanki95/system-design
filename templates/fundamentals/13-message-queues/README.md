# Message Queues

## What is a Message Queue?

A Message Queue is a communication mechanism that allows different services to communicate asynchronously by sending messages through a queue.

Instead of communicating directly, one service produces a message and another service consumes it later.

---

## Why Do We Need Message Queues?

Without a queue:

User → Server A → Server B

If Server B is slow, Server A also becomes slow.

With a queue:

User

↓

Server A

↓

Message Queue

↓

Server B

Server A responds immediately while Server B processes the task asynchronously.

---

## Advantages

- Loose Coupling
- Better Scalability
- Fault Tolerance
- Asynchronous Processing

---

## Popular Technologies

- Apache Kafka
- RabbitMQ
- Amazon SQS

---

## Real World Examples

- Sending Emails
- Order Processing
- Notifications
- Payment Processing

---

## Spring Boot Connection

Spring Boot integrates with Kafka and RabbitMQ for event-driven communication.

---

## Interview Questions

1. What is a Message Queue?
2. Why use Kafka?
3. Kafka vs RabbitMQ?
4. What is asynchronous communication?
5. When should you avoid a queue?

---

## Key Takeaways

- Enables asynchronous communication.
- Improves scalability.
- Decouples services.