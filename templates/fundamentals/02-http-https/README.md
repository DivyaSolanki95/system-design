# HTTP & HTTPS

## 📖 What is HTTP?

HTTP (HyperText Transfer Protocol) is the communication protocol used by clients and servers to exchange information over the internet.

It defines a standard set of rules for how requests are sent from a client and how responses are returned by a server.

Simply put, HTTP is the language that allows your browser or mobile application to communicate with a web server.

---

# Why Do We Need HTTP?

Imagine a client and a server speaking different languages.

The client would not understand the server, and the server would not understand the client.

HTTP provides a common language that both sides follow.

---

# Real World Example

When you search:

Spring Boot Tutorial

The browser sends an HTTP request to YouTube.

The YouTube server processes the request, retrieves matching videos from the database, and returns an HTTP response.

Flow:

User
↓

Browser (Client)

↓

HTTP Request

↓

YouTube Server

↓

Database

↓

HTTP Response

↓

Browser

↓

User

---

# Structure of an HTTP Request

An HTTP request generally contains:

- HTTP Method
- URL
- Headers
- Body (Optional)

Example:

GET /users

---

# Structure of an HTTP Response

An HTTP response generally contains:

- Status Code
- Headers
- Response Body

Example:

HTTP/1.1 200 OK

{
  "message": "Success"
}

---

# Common HTTP Methods

| Method | Purpose |
|---------|----------|
| GET | Retrieve data |
| POST | Create new data |
| PUT | Replace existing data |
| PATCH | Partially update data |
| DELETE | Remove data |

---

# What is HTTPS?

HTTPS (HyperText Transfer Protocol Secure) is the secure version of HTTP.

HTTPS encrypts the communication between the client and server using SSL/TLS, protecting sensitive information such as passwords, banking details, and personal data while it travels across the internet.

---

# HTTP vs HTTPS

| HTTP | HTTPS |
|------|-------|
| Not encrypted | Encrypted |
| Less secure | More secure |
| Uses Port 80 | Uses Port 443 |
| Suitable for non-sensitive communication | Required for sensitive communication |

---

# Why is HTTPS Important?

HTTPS protects users from:

- Password theft
- Data interception
- Session hijacking
- Man-in-the-middle attacks

Most modern websites use HTTPS by default because it provides confidentiality, integrity, and authentication.

---

# Spring Boot Connection

Whenever we build REST APIs using Spring Boot, our APIs communicate over HTTP.

In production environments, these APIs should always be served over HTTPS to ensure secure communication between clients and servers.

---

# Interview Questions

1. What is HTTP?
2. What is HTTPS?
3. Difference between HTTP and HTTPS?
4. Explain the request-response cycle.
5. What are the common HTTP methods?
6. Why should production APIs use HTTPS?

---

# Key Takeaways

- HTTP is the communication protocol between client and server.
- HTTPS is the secure version of HTTP.
- Clients send requests.
- Servers process requests and return responses.
- Modern applications should always use HTTPS.