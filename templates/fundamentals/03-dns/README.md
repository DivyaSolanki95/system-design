# DNS (Domain Name System)

## 📖 What is DNS?

DNS (Domain Name System) is the internet's phonebook.

Humans remember domain names like:

google.com

youtube.com

github.com

Computers communicate using IP addresses such as:

142.250.183.78

DNS translates a human-readable domain name into an IP address so that the client can connect to the correct server.

---

# Why Do We Need DNS?

Imagine remembering the IP address of every website you visit.

Instead of typing:

142.250.183.78

you simply type:

google.com

DNS performs the lookup behind the scenes.

---

# DNS Lookup Flow

User

↓

Browser

↓

DNS Resolver

↓

DNS Server

↓

IP Address Returned

↓

Browser Connects to Server

↓

Website Opens

---

# Real World Example

You type:

https://www.youtube.com

The browser asks the DNS server:

"What is the IP address of youtube.com?"

The DNS server responds with an IP address.

The browser then sends an HTTPS request to that IP address.

---

# Benefits of DNS

- Easy to remember website names
- Faster access using DNS caching
- Scalable internet infrastructure
- Domain names remain the same even if server IPs change

---

# Spring Boot Connection

When your Spring Boot application is deployed to a cloud platform, users access it using a domain name rather than an IP address.

Example:

https://api.myapp.com

instead of

http://34.120.88.12

---

# Interview Questions

1. What is DNS?
2. Why is DNS required?
3. What happens when you type google.com into your browser?
4. Can one domain have multiple IP addresses?
5. What is DNS caching?

---

# Key Takeaways

- DNS converts domain names into IP addresses.
- Computers communicate using IP addresses.
- Humans use domain names.
- DNS acts as the internet's phonebook.