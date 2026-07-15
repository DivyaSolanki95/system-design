# System Design Interview Framework

## Why Do We Need a Framework?

System design interviews are not about finding one correct architecture.

Interviewers evaluate how you think, communicate, identify trade-offs, and justify your design decisions.

A structured framework helps you approach any system design problem confidently.

---

# Step 1 – Clarify Requirements

Ask questions before designing.

Examples:

- Who are the users?
- Read-heavy or write-heavy?
- Expected scale?
- Functional requirements?
- Non-functional requirements?

---

# Step 2 – Estimate Scale

Estimate:

- Daily Active Users
- Requests per Second (RPS)
- Storage Requirements
- Bandwidth

Approximate calculations are acceptable.

---

# Step 3 – Design APIs

Example:

POST /shorten

GET /{shortCode}

Define inputs and outputs.

---

# Step 4 – Design the Database

Choose:

- SQL or NoSQL
- Tables or Collections
- Indexes
- Relationships

Explain your choices.

---

# Step 5 – High-Level Design

Draw the architecture.

Example:

Client

↓

Load Balancer

↓

Application Servers

↓

Cache

↓

Database

---

# Step 6 – Identify Bottlenecks

Consider:

- Database overload
- Cache misses
- Network latency
- Single Point of Failure

---

# Step 7 – Scale the System

Discuss:

- Load Balancers
- Replication
- Sharding
- Caching
- CDN
- Message Queues

---

# Step 8 – Discuss Trade-offs

No design is perfect.

Explain why you chose one approach over another.

Interviewers value reasoning more than memorized architectures.

---

# Interview Questions

1. How do you start a system design interview?
2. What should be discussed before drawing the architecture?
3. Why are trade-offs important?

---

# Key Takeaways

A structured approach leads to clear, confident system design discussions.