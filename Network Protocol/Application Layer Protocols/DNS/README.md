# Domain Name System (DNS)
# 📖 Overview

The **Domain Name System (DNS)** is a protocol that translates **human-readable domain names** into **IP addresses**.

Humans find it easier to remember names like **google.com** or **openai.com**, whereas computers communicate using numerical IP addresses such as **142.250.183.78** or **172.217.160.46**.

DNS acts like the **phonebook of the Internet**, allowing users to access websites using easy-to-remember names instead of numeric IP addresses.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What is DNS?
- Why DNS is needed
- How DNS works
- Types of DNS servers
- Advantages and limitations
- Real-world applications

---

# 📑 Table of Contents

- What is DNS?
- Why is DNS Needed?
- How DNS Works
- Types of DNS Servers
- Default Ports
- Advantages
- Limitations
- Real-World Applications
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is DNS?

**DNS (Domain Name System)** is a distributed naming system that converts domain names into IP addresses.

For example:

```text
www.google.com
        │
        ▼
142.250.xxx.xxx
```

Without DNS, users would need to remember the IP address of every website they wanted to visit.

---

# ❓ Why is DNS Needed?

DNS is important because it:

- Converts domain names into IP addresses.
- Eliminates the need to memorize IP addresses.
- Makes Internet browsing user-friendly.
- Supports scalable Internet communication.
- Enables websites to change IP addresses without affecting users.

---

# ⚙️ How DNS Works

When a user enters a domain name into a web browser:

1. The browser checks its local DNS cache.
2. If the address is not found, the request is sent to a DNS Resolver.
3. The resolver contacts the appropriate DNS servers.
4. The IP address is returned.
5. The browser connects to the destination server using that IP address.

---

# 🗂️ Types of DNS Servers

## 1. DNS Resolver

Receives DNS queries from client devices and finds the required IP address.

---

## 2. Root DNS Server

Directs the resolver to the appropriate Top-Level Domain (TLD) server.

---

## 3. Top-Level Domain (TLD) Server

Manages domain extensions such as:

- .com
- .org
- .net
- .edu

It directs the resolver to the authoritative name server.

---

## 4. Authoritative Name Server

Stores the actual DNS records for a domain and returns the correct IP address.

---

# 📡 Default Ports

| Protocol | Port | Purpose |
|----------|-----:|----------|
| UDP | 53 | Standard DNS queries |
| TCP | 53 | Zone transfers and large DNS responses |

Most DNS lookups use **UDP** because it is faster.

---

# 📋 Common DNS Record Types

| Record | Purpose |
|---------|----------|
| A | Maps a domain to an IPv4 address |
| AAAA | Maps a domain to an IPv6 address |
| CNAME | Creates an alias for another domain |
| MX | Specifies the mail server for a domain |
| NS | Identifies the authoritative name server |
| TXT | Stores text information (verification, security, etc.) |

---

# ✅ Advantages

- Easy-to-remember website names.
- Faster Internet access through caching.
- Supports large-scale Internet communication.
- Allows websites to change IP addresses without changing the domain name.
- Highly scalable and distributed.

---

# ❌ Limitations

- DNS server failures can interrupt name resolution.
- Incorrect DNS records can prevent access to websites.
- DNS attacks (such as cache poisoning or spoofing) can redirect users to malicious sites.

---

# 🌍 Real-World Applications

DNS is used whenever you:

- Browse websites
- Send emails
- Access cloud services
- Stream online content
- Use mobile applications
- Connect to online games

---

# 📷 Diagram

![DNS](https://github.com/varun-kumar-sec/networking-notes/blob/main/Network%20Protocol/Image/DNS.png?raw=true)

---

# 🎤 Interview Questions

### Beginner

- What is DNS?
- Why is DNS used?
- Which ports does DNS use?
- What is the purpose of a DNS Resolver?

### Intermediate

- Explain the DNS resolution process.
- Why does DNS primarily use UDP?
- What is the purpose of an MX record?
- Differentiate between A and AAAA records.

---

# 📌 Key Takeaways

- DNS stands for **Domain Name System**.
- It converts domain names into IP addresses.
- DNS primarily uses **UDP Port 53** and **TCP Port 53**.
- DNS consists of multiple server types, including Resolver, Root, TLD, and Authoritative servers.
- Common DNS records include **A, AAAA, CNAME, MX, NS, and TXT**.
- DNS makes Internet browsing simple by allowing users to use domain names instead of IP addresses.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- RFC 1034 – Domain Names: Concepts and Facilities
- RFC 1035 – Domain Names: Implementation and Specification
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
