# How IPv4 Addressing Works
# 📖 Overview

An IPv4 address does more than simply identify a device—it enables communication between devices across local networks and the Internet.

When a device sends data, the source and destination IPv4 addresses are included in the packet. Networking devices such as routers use these addresses to determine where the packet should be forwarded until it reaches its destination.

This process allows billions of devices around the world to communicate reliably using IPv4.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- How IPv4 communication works
- Source and destination IP addresses
- Packet forwarding
- The role of routers
- Local and remote communication
- The complete IPv4 communication process

---

# 📑 Table of Contents

- How IPv4 Works
- Source and Destination IP Addresses
- Local Communication
- Communication Across Networks
- Role of Routers
- Communication Process
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 How IPv4 Works

When one device wants to communicate with another, it creates a data packet.

This packet contains two important IPv4 addresses:

- **Source IP Address** – Identifies the sender.
- **Destination IP Address** – Identifies the receiver.

As the packet travels across the network, routers examine the destination IP address and forward the packet toward its destination.

---

# 📍 Source and Destination IP Addresses

Every IPv4 packet contains two logical addresses.

Example:

```text
Source IP:
192.168.1.10

Destination IP:
192.168.1.20
```

The source IP tells the receiver where the packet originated.

The destination IP tells the network where the packet should be delivered.

---

# 🏠 Local Communication

If both devices are connected to the same Local Area Network (LAN):

1. The sender determines that the destination is on the same network.
2. ARP is used to obtain the destination MAC address.
3. The packet is delivered directly to the destination device.

Example:

```text
Laptop
192.168.1.10

↓

Printer
192.168.1.20
```

No router is required because both devices are on the same network.

---

# 🌍 Communication Across Networks

If the destination device is located on a different network:

1. The sender creates an IP packet.
2. The packet is sent to the default gateway (router).
3. The router examines the destination IP address.
4. The packet is forwarded through one or more routers.
5. The destination network receives the packet.
6. The destination device processes the packet.

Example:

```text
Home Network

↓

Internet

↓

Office Network
```

---

# 🛣️ Role of Routers

Routers are responsible for forwarding IPv4 packets between networks.

When a router receives a packet, it:

- Reads the destination IP address.
- Checks its routing table.
- Determines the best path.
- Forwards the packet to the next network.

Routers repeat this process until the packet reaches its destination.

---

# 🔄 IPv4 Communication Process

The complete process is as follows:

1. A sender creates data.
2. The sender adds the source and destination IP addresses.
3. If the destination is on the same LAN, the packet is delivered directly.
4. If the destination is on another network, the packet is sent to the router.
5. Routers forward the packet toward the destination.
6. The destination device receives and processes the packet.

---

# 📷 Diagram

Save the diagram as:

```text
images/ipv4-communication.png
```

Recommended diagram:

```text
Computer A
192.168.1.10
      │
      ▼
   Router
      │
      ▼
   Internet
      │
      ▼
   Router
      │
      ▼
Computer B
10.0.0.20
```

Suggested sources:

- https://commons.wikimedia.org/wiki/Category:Internet_Protocol
- https://en.wikipedia.org/wiki/Internet_Protocol

---

# 🎤 Interview Questions

### Beginner

- How does IPv4 communication work?
- What is the purpose of the source IP address?
- What is the purpose of the destination IP address?
- When is a router required?

### Intermediate

- Explain the IPv4 communication process.
- How do routers use IPv4 addresses?
- What happens if the destination device is on another network?
- Why are source and destination IP addresses required?

---

# 📌 Key Takeaways

- IPv4 communication is based on **logical addressing**.
- Every packet contains a **source IP address** and a **destination IP address**.
- Devices on the same network communicate directly after address resolution.
- Communication between different networks requires routers.
- Routers forward packets by examining the destination IP address and selecting the appropriate path.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- RFC 791 – Internet Protocol (IPv4)
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
