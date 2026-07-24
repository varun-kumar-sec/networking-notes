# IPv4 (Internet Protocol Version 4)
# 📖 Overview

**IPv4 (Internet Protocol Version 4)** is the fourth version of the Internet Protocol and is the most widely used addressing system in computer networks.

It assigns a **32-bit logical address** to every device connected to a network, allowing devices to identify each other and communicate over local networks and the Internet.

Although IPv6 was developed to overcome IPv4 address limitations, IPv4 remains the dominant protocol in most networks today.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What is IPv4?
- Why IPv4 was developed
- IPv4 address format
- Structure of an IPv4 address
- Characteristics of IPv4
- Advantages and limitations

---

# 📑 Table of Contents

- What is IPv4?
- Why is IPv4 Needed?
- IPv4 Address Format
- Structure of an IPv4 Address
- Characteristics of IPv4
- Advantages
- Limitations
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is IPv4?

**IPv4 (Internet Protocol Version 4)** is the fourth version of the Internet Protocol that provides logical addressing for devices connected to a network.

Every device using IPv4 receives a **32-bit address**, allowing routers to identify the source and destination of data packets.

An example IPv4 address is:

```text
192.168.1.10
```

---

# ❓ Why is IPv4 Needed?

IPv4 is used to:

- Uniquely identify devices on a network.
- Enable communication between devices.
- Support routing across multiple networks.
- Allow data packets to reach the correct destination.

---

# 🧩 IPv4 Address Format

An IPv4 address consists of:

- **32 bits**
- Divided into **4 octets**
- Each octet contains **8 bits**
- Octets are separated by periods (.)

Example:

```text
192.168.1.10
```

Binary representation:

```text
11000000.10101000.00000001.00001010
```

---

# 🏗️ Structure of an IPv4 Address

An IPv4 address contains **four octets**.

Example:

```text
192 . 168 . 1 . 10
 │      │     │    │
Octet Octet Octet Octet
```

Each octet:

- Contains **8 bits**
- Has a decimal value between **0 and 255**

Therefore:

```text
Minimum Value: 0
Maximum Value: 255
```

---

# ⭐ Characteristics of IPv4

IPv4 has the following characteristics:

- 32-bit addressing.
- Four decimal octets.
- Dot-decimal notation.
- Supports approximately **4.3 billion unique addresses**.
- Uses logical addressing.
- Widely supported across networking devices.

---

# ✅ Advantages

- Simple and easy to understand.
- Widely deployed worldwide.
- Supported by almost all networking devices.
- Efficient for small and medium-sized networks.

---

# ❌ Limitations

- Limited address space.
- IPv4 addresses are becoming exhausted.
- Requires techniques such as NAT to conserve addresses.
- Less scalable than IPv6.

---

# 📷 Diagram

Save the diagram as:

```text
images/ipv4-format.png
```

Recommended diagram:

```text
IPv4 Address

192 . 168 . 1 . 10
 │      │     │    │
8 bits 8 bits 8 bits 8 bits

Total = 32 bits
```

Suggested sources:

- https://commons.wikimedia.org/wiki/Category:IPv4
- https://en.wikipedia.org/wiki/IPv4

---

# 🎤 Interview Questions

### Beginner

- What is IPv4?
- How many bits are in an IPv4 address?
- How many octets are present in an IPv4 address?
- What is the decimal range of each octet?

### Intermediate

- Explain the structure of an IPv4 address.
- Why was IPv6 introduced?
- Approximately how many unique IPv4 addresses exist?
- Why is IPv4 still widely used?

---

# 📌 Key Takeaways

- IPv4 stands for **Internet Protocol Version 4**.
- It uses **32-bit logical addresses**.
- An IPv4 address consists of **4 octets**, each containing **8 bits**.
- Each octet ranges from **0 to 255**.
- IPv4 uses **dot-decimal notation**.
- Although IPv6 exists, IPv4 remains the most widely deployed version of the Internet Protocol.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- RFC 791 – Internet Protocol (IPv4)
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
