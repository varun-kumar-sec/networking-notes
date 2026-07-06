# Router
# 📖 Overview

A **Router** is a Layer 3 (Network Layer) networking device that connects multiple networks and forwards data packets between them using **IP addresses**.

Unlike switches, which forward frames based on MAC addresses within a Local Area Network (LAN), routers examine the destination IP address and determine the best path for forwarding packets to another network.

Routers are commonly used to connect Local Area Networks (LANs) to Wide Area Networks (WANs), such as the Internet.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What a Router is
- Why Routers are required
- How a Router works
- Routing Process
- Routing Table
- Default Gateway
- OSI Layer
- Advantages and disadvantages
- Security considerations

---

# 📑 Table of Contents

- What is a Router?
- Why is a Router Required?
- How Does a Router Work?
- Routing Table
- Default Gateway
- OSI Layer
- Types of Routers
- Advantages
- Disadvantages
- Real-world Applications
- Security Perspective
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is a Router?

A **Router** is a networking device that connects different networks and forwards data packets between them using **IP addresses**.

Its primary function is to determine the best available path for packets to reach their destination.

Unlike a Switch, which works only within a Local Area Network, a Router enables communication between completely different networks.

---

# ❓ Why is a Router Required?

A Router is required because:

- It connects different networks.
- It enables Internet access.
- It forwards packets using IP addresses.
- It determines the optimal route for packet delivery.
- It prevents unnecessary traffic between networks.

Without a Router, communication would be limited to devices within the same network.

---

# ⚙️ How Does a Router Work?

The working process of a router is as follows:

1. A device sends a packet destined for another network.
2. The packet reaches the Router.
3. The Router reads the destination IP address.
4. It checks its Routing Table.
5. The Router determines the best available path.
6. The packet is forwarded to the next network until it reaches its destination.

Unlike switches, routers make forwarding decisions based on **IP addresses** rather than MAC addresses.

---

# 🗺 Routing Table

A **Routing Table** is a database maintained by the router that contains information about available networks and the paths used to reach them.

A typical routing table includes:

- Destination Network
- Next Hop
- Interface
- Metric

The router consults this table whenever it forwards a packet.

---

# 🚪 Default Gateway

In most Local Area Networks, the Router acts as the **Default Gateway**.

When a computer wants to communicate with a device outside its own network, it forwards the packet to the Router.

Example:

```
PC

IP Address: 192.168.1.10

Default Gateway: 192.168.1.1
```

If the destination belongs to another network, the Router forwards the packet accordingly.

---

# 📡 OSI Layer

A Router primarily operates at:

## **Layer 3 – Network Layer**

At this layer, the Router processes:

- IP Addresses
- Routing Information
- Network Paths

Unlike switches, routers do not forward packets using MAC addresses as their primary decision-making mechanism.

---

# 🧭 Types of Routers

Common types of routers include:

## 1. Wired Router

- Uses Ethernet cables
- Common in enterprise environments
- Stable and high-speed communication

---

## 2. Wireless Router

- Provides Wi-Fi connectivity
- Common in homes and offices
- Connects both wired and wireless devices

---

## 3. Core Router

- Used within Internet Service Providers (ISPs)
- Handles very high-speed network traffic
- Connects backbone networks

---

## 4. Edge Router

- Located at the boundary of a network
- Connects internal networks to external networks such as the Internet

---

# 🌍 Real-World Applications

Routers are commonly used in:

- Home Networks
- Office Networks
- Data Centers
- Internet Service Providers (ISPs)
- Cloud Infrastructure
- Enterprise Networks

Almost every network that requires Internet connectivity uses a router.

---

# ✅ Advantages

- Connects multiple networks
- Supports Internet connectivity
- Determines the best routing path
- Reduces unnecessary network traffic
- Supports security features
- Enables communication between different IP networks

---

# ❌ Disadvantages

- More expensive than switches
- Configuration can be complex
- Packet processing introduces slight latency
- Requires proper routing configuration

---

# 🛡 Security Perspective

Modern routers provide several security features, including:

- Network Address Translation (NAT)
- Access Control Lists (ACLs)
- Firewall functionality
- VPN support
- Packet filtering

However, routers may also be targeted by attacks such as:

- Route Poisoning
- Routing Table Manipulation
- DDoS Attacks
- Default Credential Attacks

Proper configuration and regular firmware updates are essential to securing routers.

---

# 📷 Diagram

Save as:

```
images/router-working.png
```

Recommended diagrams:

- https://commons.wikimedia.org/wiki/File:Router_architecture.svg
- https://en.wikipedia.org/wiki/Router_(computing)

---

# 🎤 Interview Questions

### Beginner

- What is a Router?
- Which OSI layer does a Router operate on?
- What is the purpose of a Router?
- What information does a Router use to forward packets?
- What is a Default Gateway?

### Intermediate

- What is a Routing Table?
- What is the difference between a Router and a Switch?
- Why does a Router operate at Layer 3?
- Explain the packet forwarding process.
- What security features are commonly available on modern routers?

---

# 📌 Key Takeaways

- A Router is a Layer 3 networking device.
- It forwards packets using IP addresses.
- Routers connect different networks.
- Every router maintains a Routing Table.
- Routers commonly act as the Default Gateway.
- Modern routers also provide security features such as NAT, firewalls, VPNs, and ACLs.

---

# 📚 References

- Cisco Networking Academy
- CompTIA Network+
- RFC 1812 – Requirements for IP Version 4 Routers
- Microsoft Learn
