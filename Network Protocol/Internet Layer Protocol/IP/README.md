# Internet Protocol (IP)
# 📖 Overview

The **Internet Protocol (IP)** is the core protocol responsible for delivering data packets from a source device to a destination device across one or more networks.

IP provides **logical addressing** and **routing**, allowing devices connected to different networks to communicate with each other.

Unlike Transport Layer protocols such as TCP, IP does not guarantee reliable delivery. Its responsibility is simply to move packets toward their destination using IP addresses.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What is IP?
- Why IP is used
- How IP works
- IPv4 and IPv6
- Key features of IP
- Advantages and limitations
- Real-world applications

---

# 📑 Table of Contents

- What is IP?
- Why is IP Needed?
- How IP Works
- IPv4 and IPv6
- Features of IP
- Advantages
- Limitations
- Real-World Applications
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is IP?

**IP (Internet Protocol)** is a protocol used to identify devices and route data packets between them.

Each device connected to a network is assigned a unique **IP address**, which allows routers and other networking devices to determine where packets should be delivered.

IP focuses on:

- Logical addressing
- Packet forwarding
- Routing
- Inter-network communication

---

# ❓ Why is IP Needed?

IP is important because it:

- Provides unique logical addresses.
- Enables communication between different networks.
- Allows routers to forward packets.
- Supports communication across the Internet.
- Makes large-scale networking possible.

---

# ⚙️ How IP Works

The communication process generally follows these steps:

1. A sender creates data to be transmitted.
2. The data is encapsulated into an IP packet.
3. The source and destination IP addresses are added.
4. Routers examine the destination IP address.
5. The packet is forwarded through one or more networks.
6. The packet reaches the destination device.

---

# 🌍 IPv4 and IPv6

## IPv4

- Uses **32-bit addresses**
- Example:

```text
192.168.1.10
```

- Most widely deployed version of IP.

---

## IPv6

- Uses **128-bit addresses**
- Example:

```text
2001:db8::1
```

- Designed to overcome IPv4 address exhaustion.
- Provides a significantly larger address space.

---

# ⭐ Features of IP

The Internet Protocol provides several important features:

- Logical addressing.
- Packet routing.
- Connectionless communication.
- Best-effort delivery.
- Scalability for large networks.
- Supports communication across multiple interconnected networks.

---

# ✅ Advantages

- Enables global Internet communication.
- Supports communication between different networks.
- Scalable for small and large environments.
- Independent of the underlying physical network technology.
- Widely supported across networking devices.

---

# ❌ Limitations

- Does not guarantee packet delivery.
- Does not provide error recovery.
- Does not guarantee packet ordering.
- Does not provide flow control.
- Relies on higher-layer protocols such as TCP when reliable communication is required.

---

# 🌍 Real-World Applications

IP is used in:

- Internet communication
- Local Area Networks (LANs)
- Wide Area Networks (WANs)
- Cloud computing
- Mobile networks
- Enterprise networks
- Home networking

---

# 📷 Diagram

![IP](https://github.com/varun-kumar-sec/networking-notes/blob/main/Network%20Protocol/Image/ip.jpg?raw=true)

---

# 🎤 Interview Questions

### Beginner

- What is Internet Protocol (IP)?
- Which OSI layer uses IP?
- What is the primary purpose of IP?
- What is the difference between IPv4 and IPv6?

### Intermediate

- Explain how IP works.
- Why is IP called a connectionless protocol?
- Does IP guarantee packet delivery?
- What is the role of routers in IP communication?
- Why was IPv6 introduced?

---

# 📌 Key Takeaways

- IP stands for **Internet Protocol**.
- It operates at the **Internet Layer (TCP/IP)** and **Network Layer (OSI)**.
- IP provides **logical addressing** and **routing**.
- It is a **connectionless** and **best-effort** protocol.
- The two major versions are **IPv4** and **IPv6**.
- IP is responsible for delivering packets between networks but does not guarantee reliable delivery.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- RFC 791 – Internet Protocol (IPv4)
- RFC 8200 – Internet Protocol Version 6 (IPv6)
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
