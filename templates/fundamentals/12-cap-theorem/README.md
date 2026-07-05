# CAP Theorem

## What is CAP Theorem?

CAP Theorem states that a distributed system can guarantee only two out of the following three properties at the same time.

---

## C — Consistency

Every user sees the same data.

---

## A — Availability

Every request receives a response.

---

## P — Partition Tolerance

The system continues to work even if network failures occur.

---

## Trade-offs

CP Systems

Consistency + Partition Tolerance

Example:

MongoDB (configurable depending on setup)

---

AP Systems

Availability + Partition Tolerance

Example:

Cassandra

---

CA Systems

Possible only when there is no network partition.

---

## Interview Questions

1. Explain CAP Theorem.
2. Why can't distributed systems guarantee all three?
3. Difference between CP and AP?