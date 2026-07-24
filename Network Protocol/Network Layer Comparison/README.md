# Network Layer Protocol Comparison
# 📖 Overview

Network Layer protocols are responsible for enabling communication between devices by providing logical addressing, routing, and address resolution.

Although **ARP** and **IP** work together, they serve different purposes.

- **IP** identifies devices and routes packets between networks.
- **ARP** discovers the MAC address associated with an IPv4 address within a local network.

Understanding their differences helps explain how devices successfully communicate over Ethernet networks.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- The differences between ARP and IP.
- The purpose of each protocol.
- Where each protocol is used.
- When each protocol is required.

---

# 📑 Table of Contents

- Quick Comparison
- Feature Comparison
- When to Use Each Protocol
- Interview Questions
- Key Takeaways
- References

---

# ⚖️ Quick Comparison

| Protocol | Full Form | Primary Purpose |
|----------|-----------|-----------------|
| ARP | Address Resolution Protocol | Maps an IPv4 address to a MAC address |
| IP | Internet Protocol | Provides logical addressing and routes packets between networks |

---

# 📊 Feature Comparison

| Feature | ARP | IP |
|---------|-----|----|
| OSI Layer | Works between Data Link and Network Layers | Network Layer |
| TCP/IP Layer | Internet Layer (supports local communication) | Internet Layer |
| Purpose | Resolve MAC address from an IPv4 address | Deliver packets between devices and networks |
| Uses Addresses | IPv4 Address and MAC Address | IPv4 or IPv6 Address |
| Communication Scope | Local Area Network (LAN) only | Local and remote networks |
| Routing | No | Yes |
| Packet Forwarding | No | Yes |
| Broadcast Support | ARP Request is broadcast | No |
| Connection Type | Connectionless | Connectionless |
| Address Resolution | Yes | No |
| Common Devices | Hosts, Routers, Switches | Hosts, Routers |

---

# 🧩 How They Work Together

Suppose **Computer A** wants to send data to **Computer B** on the same LAN.

### Step 1

Computer A knows the destination **IP address**.

↓

### Step 2

It uses **ARP** to discover the destination **MAC address**.

↓

### Step 3

The MAC address is returned in an ARP Reply.

↓

### Step 4

The Ethernet frame is created using the discovered MAC address.

↓

### Step 5

The IP packet is delivered to the destination device.

---

# 📌 When to Use Each Protocol

### Use ARP when:

- You know the destination IPv4 address.
- You need the destination MAC address.
- Communication is occurring within a LAN.

---

### Use IP when:

- Sending packets across networks.
- Routing data through routers.
- Communicating over the Internet.
- Identifying devices using logical addresses.

---

# 🎤 Interview Questions

### Beginner

- What is the purpose of ARP?
- What is the purpose of IP?
- Which protocol performs routing?
- Which protocol resolves MAC addresses?

### Intermediate

- Explain how ARP and IP work together.
- Why is ARP needed before Ethernet communication?
- Can IP function without ARP in an IPv4 Ethernet LAN?
- Why is ARP limited to local networks?

---

# 📌 Key Takeaways

- **ARP** maps an **IPv4 address** to a **MAC address**.
- **IP** provides **logical addressing** and **routing**.
- ARP works only within a **Local Area Network (LAN)**.
- IP enables communication across **multiple interconnected networks**.
- ARP and IP complement each other to ensure successful packet delivery in IPv4 Ethernet networks.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- RFC 826 – Address Resolution Protocol
- RFC 791 – Internet Protocol (IPv4)
- RFC 8200 – Internet Protocol Version 6 (IPv6)
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
