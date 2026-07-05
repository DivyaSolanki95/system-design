# IP Address & Ports

## 📖 What is an IP Address?

An IP (Internet Protocol) Address is a unique numerical address assigned to every device connected to a network.

Just like every house has a unique address, every device on the internet has an IP address.

Example:

192.168.1.10

142.250.183.78

Without an IP address, devices cannot communicate over a network.

---

# Why Do We Need an IP Address?

The internet needs to know where data should go.

When you request youtube.com, DNS converts the domain name into an IP address.

The browser then communicates with that IP address.

---

# Types of IP Addresses

## IPv4

Example:

192.168.1.10

Uses 32 bits.

---

## IPv6

Example:

2001:db8:85a3::8a2e:370:7334

Uses 128 bits.

Designed because IPv4 addresses are limited.

---

# What is a Port?

A port identifies a specific application or service running on a device.

Think of:

IP Address = Apartment Building

Port = Apartment Number

The IP tells us which building.

The port tells us which apartment.

---

# Common Ports

| Port | Service |
|------|----------|
| 80 | HTTP |
| 443 | HTTPS |
| 22 | SSH |
| 3306 | MySQL |
| 5432 | PostgreSQL |
| 6379 | Redis |
| 8080 | Spring Boot |

---

# Real World Example

You open:

https://google.com

↓

DNS returns an IP address.

↓

Browser connects to that IP using Port 443.

↓

Google Server returns the webpage.

---

# Spring Boot Connection

When you run a Spring Boot application locally:

http://localhost:8080

8080 is the default port.

You can change it in:

application.properties

server.port=9090

---

# Interview Questions

1. What is an IP Address?
2. What is a Port?
3. Difference between IPv4 and IPv6?
4. Why do we need ports?
5. What port does HTTPS use?

---

# Key Takeaways

- Every device has an IP address.
- Every service listens on a port.
- IP identifies the machine.
- Port identifies the application.