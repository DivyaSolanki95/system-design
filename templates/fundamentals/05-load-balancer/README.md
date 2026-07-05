# Load Balancer

## 📖 What is a Load Balancer?

A Load Balancer is a component that distributes incoming client requests across multiple servers.

Instead of sending all traffic to one server, it spreads the load to ensure high availability, scalability, and better performance.

---

# Why Do We Need a Load Balancer?

Imagine an application with only one server.

```
Users
   |
   v
Server
```

If 1 million users visit simultaneously:

- Server becomes overloaded.
- Response time increases.
- The server may crash.

A Load Balancer solves this problem by distributing requests.

```
          Users
             |
             v
      Load Balancer
       /     |     \
      /      |      \
Server 1  Server 2  Server 3
```

---

# Benefits

- High Availability
- Scalability
- Fault Tolerance
- Better Performance

---

# Load Balancing Algorithms

### Round Robin

Requests are distributed one by one.

Example:

Request 1 → Server 1

Request 2 → Server 2

Request 3 → Server 3

Request 4 → Server 1

---

### Least Connections

The request goes to the server with the fewest active connections.

---

### Weighted Round Robin

More powerful servers receive more requests.

---

# Health Checks

The Load Balancer continuously checks whether servers are alive.

If Server 2 crashes:

```
Load Balancer

✓ Server 1

✗ Server 2

✓ Server 3
```

Traffic automatically goes only to Server 1 and Server 3.

---

# Spring Boot Connection

Suppose we deploy three Spring Boot instances.

Instead of:

Client → Server 1

We have:

Client

↓

Load Balancer

↓

Spring Boot Instance 1

Spring Boot Instance 2

Spring Boot Instance 3

---

# Interview Questions

1. Why do we need a Load Balancer?
2. Difference between Round Robin and Least Connections?
3. What happens if a server crashes?
4. Can a Load Balancer become a single point of failure?
5. What are health checks?

---

# Key Takeaways

- Distributes requests
- Prevents server overload
- Improves availability
- Enables horizontal scaling