# Database Indexing

## 📖 What is Database Indexing?

A database index is a data structure that helps the database find rows much faster without scanning the entire table.

Think of it like the index of a book. Instead of reading every page, you jump directly to the page you need.

---

# Why Do We Need Indexing?

Imagine a Users table with 10 million records.

Without an index:

SELECT * FROM users WHERE email = 'divya@gmail.com';

The database scans every row.

This is called a Full Table Scan.

With an index on the email column:

The database directly locates the matching record.

---

# Example

Without Index

Time Complexity:

O(n)

Database checks every row.

---

With Index

Time Complexity (typically):

O(log n)

Database uses a B-Tree index to quickly locate the record.

---

# Advantages

- Faster SELECT queries
- Reduced query execution time
- Better application performance

---

# Disadvantages

- Extra storage required
- INSERT, UPDATE, DELETE become slightly slower because indexes must also be updated

---

# When Should You Create an Index?

Create indexes on:

- Primary Keys
- Foreign Keys
- Frequently searched columns
- Columns used in WHERE clauses
- Columns used in JOIN operations

Avoid indexing:

- Very small tables
- Frequently updated columns (unless necessary)
- Low-cardinality columns (like a boolean field)

---

# Spring Boot Connection

When using Spring Data JPA, indexes are usually created at the database level.

Example:

Searching users by email.

Without an index:

Slow query.

With an index:

Fast query.

---

# Interview Questions

1. What is an index?
2. Why are indexes used?
3. What is a Full Table Scan?
4. Can too many indexes hurt performance?
5. Which columns should be indexed?

---

# Key Takeaways

- Indexes improve read performance.
- Indexes consume additional storage.
- Too many indexes can slow down writes.
- Proper indexing is essential for scalable applications.