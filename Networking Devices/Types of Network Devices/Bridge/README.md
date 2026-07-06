# Bridge
# 📖 Overview

A **Bridge** is a Layer 2 (Data Link Layer) networking device that connects two or more LAN segments and forwards data based on **MAC addresses**.

Unlike a Hub, which broadcasts every frame to all connected devices, a Bridge intelligently decides whether to forward or filter a frame based on the destination MAC address. This reduces unnecessary network traffic and minimizes collisions.

Although bridges are rarely used today, they introduced the concept of intelligent frame forwarding, which later evolved into modern network switches.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What a Bridge is
- Why a Bridge is required
- How a Bridge works
- MAC Address Learning
- Collision Domains
- Broadcast Domains
- OSI Layer
- Advantages and disadvantages
- Security considerations

---

# 📑 Table of Contents

- What is a Bridge?
- Why is a Bridge Required?
- How Does a Bridge Work?
- MAC Address Learning
- Collision Domain
- Broadcast Domain
- OSI Layer
- Types of Bridge
- Advantages
- Disadvantages
- Real-world Applications
- Security Perspective
- Interview Questions
- Key Takeaways
- References

---

# 🌉 What is a Bridge?

A **Bridge** is a Layer 2 networking device that connects multiple LAN segments and forwards Ethernet frames based on **MAC addresses**.

Instead of sending every frame to all connected devices, a bridge checks the destination MAC address and forwards the frame only if necessary.

This makes communication much more efficient than a Hub.

---

# ❓ Why is a Bridge Required?

As networks grow larger, using a Hub creates:

- Excessive broadcasts
- Frequent collisions
- Reduced network performance

A Bridge helps by:

- Dividing a network into multiple segments
- Reducing collisions
- Filtering unnecessary traffic
- Improving overall network efficiency

---

# ⚙️ How Does a Bridge Work?

The working process of a bridge is as follows:

1. A frame arrives at one of the bridge's ports.
2. The bridge examines the **source MAC address** and stores it in its MAC Address Table.
3. It checks the **destination MAC address**.
4. If the destination is on another segment, the frame is forwarded.
5. If the destination is on the same segment, the frame is filtered and not forwarded.

This intelligent forwarding reduces unnecessary traffic.

---

# 📘 MAC Address Learning

One of the key features of a Bridge is **MAC Address Learning**.

The bridge automatically builds a table containing:

- MAC Address
- Incoming Port

Example:

| MAC Address | Port |
|-------------|------|
| AA:BB:CC:11:22:33 | Port 1 |
| DD:EE:FF:44:55:66 | Port 2 |

Whenever a new frame arrives, the bridge updates this table automatically.

---

# 💥 Collision Domain

Unlike a Hub, a Bridge separates the network into multiple **Collision Domains**.

Example:

```
LAN 1 ---- Bridge ---- LAN 2
```

- LAN 1 has its own collision domain.
- LAN 2 has its own collision domain.

As a result, collisions occurring on one LAN do not affect the other.

---

# 📡 Broadcast Domain

A Bridge **does not** separate Broadcast Domains.

Broadcast frames are forwarded to every connected network segment.

Therefore:

- Collision Domains → Separated ✅
- Broadcast Domain → Remains the same ❌

---

# 📡 OSI Layer

A Bridge operates at:

## **Layer 2 – Data Link Layer**

At this layer, the bridge understands:

- Ethernet Frames
- MAC Addresses

It does **not** make routing decisions based on IP addresses.

---

# 📚 Types of Bridge

Common bridge types include:

## 1. Transparent Bridge

- Most common type
- Learns MAC addresses automatically
- Used in Ethernet LANs

---

## 2. Source Routing Bridge

- Used mainly in Token Ring networks
- Source device determines the path

---

## 3. Translational Bridge

- Connects different LAN technologies
- Converts frames between different network standards

---

# 🌍 Real-World Applications

Bridges were commonly used in:

- Office LAN segmentation
- Campus networks
- Legacy Ethernet environments

Today, their functionality is almost entirely provided by **Switches**.

---

# ✅ Advantages

- Reduces collisions
- Filters unnecessary traffic
- Learns MAC addresses automatically
- Improves LAN performance
- Segments networks efficiently

---

# ❌ Disadvantages

- Cannot separate broadcast domains
- Slower than modern switches
- Limited number of ports
- Mostly obsolete in modern networks

---

# 🛡 Security Perspective

A Bridge offers better security than a Hub because it forwards frames only when necessary.

However, it still cannot:

- Inspect packet contents
- Detect attacks
- Filter malicious traffic
- Block unauthorized access

Security still relies on higher-layer devices such as switches, routers, and firewalls.

---

# 📷 Diagram

![Bridge](https://github.com/varun-kumar-sec/networking-notes/blob/main/Networking%20Devices/Types%20of%20Network%20Devices/Bridge/image/Bridge.png?raw=true)

---

# 🎤 Interview Questions

### Beginner

- What is a Bridge?
- Which OSI layer does a Bridge operate on?
- What is MAC Address Learning?
- Why is a Bridge better than a Hub?
- What does a Bridge use to forward frames?

### Intermediate

- What is the difference between a Bridge and a Hub?
- Does a Bridge separate collision domains?
- Does a Bridge separate broadcast domains?
- Why have switches replaced bridges?
- Explain the forwarding process of a Bridge.

---

# 📌 Key Takeaways

- A Bridge is a Layer 2 networking device.
- It forwards frames using MAC addresses.
- Bridges learn MAC addresses automatically.
- A Bridge separates collision domains.
- A Bridge does not separate broadcast domains.
- Modern switches provide all bridge functionality with better performance.

---

# 📚 References

- Cisco Networking Academy
- CompTIA Network+
- IEEE Ethernet Standards
- Microsoft Learn
