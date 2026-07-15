# Event-Driven Architecture

## What is Event-Driven Architecture?

Event-Driven Architecture (EDA) is a software architecture where services communicate by producing and consuming events.

Instead of directly calling another service, a service publishes an event.

Interested services react to that event.

---

## Example

Customer places an order.

↓

Order Created Event

↓

Inventory Service

↓

Notification Service

↓

Analytics Service

↓

Recommendation Service

Every service works independently.

---

## Why Use Event-Driven Architecture?

- Loose Coupling
- Scalability
- Better Performance
- Asynchronous Processing

---

## Event Components

Producer

↓

Message Broker (Kafka)

↓

Consumer

---

## Real World Examples

Amazon

Order Placed

↓

Inventory Updated

↓

Email Sent

↓

Recommendation Updated

↓

Analytics Recorded

---

## Spring Boot Connection

Spring Boot integrates with Kafka and RabbitMQ to build event-driven applications.

---

## Interview Questions

1. What is Event-Driven Architecture?
2. Difference between synchronous and asynchronous communication?
3. Kafka's role in EDA?
4. Benefits of EDA?

---

## Key Takeaways

- Services communicate using events.
- Producers publish.
- Consumers subscribe.
- Kafka is a popular event broker.