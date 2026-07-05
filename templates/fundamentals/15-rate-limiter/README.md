# Rate Limiting

## What is Rate Limiting?

Rate Limiting restricts how many requests a client can make within a specific time period.

---

## Why is it Needed?

Without Rate Limiting:

- DDoS attacks
- API abuse
- Server overload

---

## Common Algorithms

- Token Bucket
- Leaky Bucket
- Fixed Window
- Sliding Window

---

## Real World Examples

- OTP APIs
- Login APIs
- Payment APIs

---

## Spring Boot Connection

Rate limiting can be implemented using Redis and Spring Boot filters.

---

## Interview Questions

1. What is Rate Limiting?
2. Why use Redis?
3. Explain Token Bucket.
4. Sliding Window vs Fixed Window?

---

## Key Takeaways

Protects APIs from abuse and improves reliability.