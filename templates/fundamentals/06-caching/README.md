# Caching

## 📖 What is Caching?

Caching is the process of storing frequently accessed data in a faster storage layer so that future requests can be served quickly without repeatedly accessing the database.

The primary goal of caching is to reduce response time, decrease database load, and improve overall application performance.

---

# Why Do We Need Caching?

Imagine a product on Amazon that receives millions of views every day.

Without caching:

Client
↓

Server
↓

Database

The database is queried every single time.

With caching:

Client
↓

Server
↓

Cache (Redis)

↓

Database (Only if data is not found)

Most requests are served directly from the cache.

---

# Cache Hit

The requested data is found in the cache.

Response is returned immediately.

---

# Cache Miss

The requested data is not found in the cache.

The server fetches it from the database, returns it to the client, and stores it in the cache for future requests.

---

# Benefits

- Faster response time
- Reduced database load
- Better scalability
- Improved user experience

---

# Popular Cache Technologies

- Redis
- Memcached

Redis is widely used because it supports multiple data structures and persistence.

---

# Real World Example

Instagram profile

The first request may access the database.

Subsequent requests are served from Redis until the cache expires.

---

# Spring Boot Connection

Spring Boot applications commonly integrate with Redis to cache frequently accessed data.

Example:

- User profile
- Product details
- Trending videos
- Frequently searched URLs

---

# Interview Questions

1. What is caching?
2. What is the difference between a cache hit and a cache miss?
3. Why is Redis commonly used for caching?
4. What happens if cached data becomes outdated?
5. Should every piece of data be cached?

---

# Key Takeaways

- Cache stores frequently accessed data.
- Cache is faster than a database.
- Cache reduces database load.
- Redis is a popular caching solution.