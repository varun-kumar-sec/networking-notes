# Hub

> **Difficulty:** Beginner  
> **Prerequisites:** Repeater  
> **Estimated Reading Time:** 10–12 Minutes

---

# 📖 Overview

A **Hub** is a basic networking device that connects multiple computers within a Local Area Network (LAN). It receives data from one connected device and broadcasts that data to **every device** connected to the hub, regardless of the intended recipient.

Since a hub blindly forwards all incoming traffic to every port, it is considered an **unintelligent networking device**.

Hubs operate only at the **Physical Layer (Layer 1)** of the OSI model and do not understand MAC addresses or IP addresses.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What a Hub is
- Why Hubs are used
- How a Hub works
- Collision Domain
- Broadcast behavior
- OSI Layer
- Advantages and disadvantages
- Security considerations

---

# 📑 Table of Contents

- What is a Hub?
- Why is a Hub Required?
- How Does a Hub Work?
- Collision in a Hub
- Collision Domain
- Broadcast Communication
- OSI Layer
- Types of Hub
- Advantages
- Disadvantages
- Real-world Applications
- Security Perspective
- Interview Questions
- Key Takeaways
- References

---

# 🔌 What is a Hub?

A **Hub** is a Physical Layer networking device that connects multiple computers into a single Local Area Network (LAN).

When a hub receives data from one device, it simply copies and forwards the data to **all available ports** except the incoming port.

It does **not** determine which device is the intended recipient.

---

# ❓ Why is a Hub Required?

A hub was originally designed to:

- Connect multiple computers in a LAN
- Extend network connectivity
- Allow devices to communicate using a common medium

Although hubs are largely obsolete today, they played an important role in early Ethernet networks.

---

# ⚙️ How Does a Hub Work?

The working process of a hub is simple:

1. A computer sends data to the hub.
2. The hub receives the incoming signal.
3. It regenerates the signal.
4. The signal is broadcast to every connected device.
5. Every device receives the data.
6. Only the intended recipient processes the data, while all other devices discard it.

Unlike switches, hubs do **not** learn device addresses or make forwarding decisions.

---

# 💥 Collision in a Hub

Since all connected devices share the same communication medium, two devices may attempt to transmit data at the same time.

When this happens, the signals interfere with each other, causing a **collision**.

A collision results in:

- Data corruption
- Packet retransmission
- Reduced network performance

This is one of the major limitations of hubs.

---

# 🌐 Collision Domain

A **Collision Domain** is a network segment where devices share the same communication channel, meaning simultaneous transmissions can result in collisions.

In a hub:

- All connected devices belong to **one single collision domain**.
- As the number of connected devices increases, the probability of collisions also increases.

This limitation was one of the primary reasons why switches replaced hubs in modern networks.

---

# 📡 Broadcast Communication

A hub broadcasts every incoming frame to **all connected devices**.

For example:

```
Computer A → Hub

          Hub
      /    |    \
     B     C     D
```

The hub forwards the data to B, C, and D simultaneously, even if only one device is the intended recipient.

This behavior increases unnecessary network traffic.

---

# 📚 Types of Hub

There are three common types of hubs:

## 1. Passive Hub

- Simply forwards incoming signals
- Does not regenerate signals
- Requires no external power for signal processing

---

## 2. Active Hub

- Regenerates and amplifies signals
- Extends communication distance
- Requires electrical power

---

## 3. Intelligent Hub

- Provides basic monitoring and management features
- Can detect simple network issues
- Mostly used in older enterprise networks

---

# 📡 OSI Layer

A Hub operates at:

## **Layer 1 – Physical Layer**

It only processes electrical or optical signals.

It does **not** understand:

- MAC Addresses
- IP Addresses
- Ethernet Frames
- Network Packets

---

# 🌍 Real-World Applications

Historically, hubs were used in:

- Small office LANs
- Computer laboratories
- Educational networks
- Testing environments

Today, hubs have almost entirely been replaced by switches due to better performance and security.

---

# ✅ Advantages

- Low cost
- Easy to install
- Connects multiple devices
- No configuration required
- Simple network expansion

---

# ❌ Disadvantages

- Creates collisions
- Broadcasts traffic to all devices
- Poor network performance
- No traffic filtering
- No security features
- Cannot identify destination devices

---

# 🛡 Security Perspective

Hubs are considered **insecure** because they broadcast every frame to every connected device.

This allows attackers to:

- Capture network traffic
- Perform packet sniffing
- Monitor other users' communication

For this reason, hubs are no longer recommended in production environments.

---

# 📷 Diagram

Save as:

```
images/hub-working.png
```

Recommended diagrams:

- https://commons.wikimedia.org/wiki/File:Ethernet_hub.svg
- https://en.wikipedia.org/wiki/Ethernet_hub

---

# 🎤 Interview Questions

### Beginner

- What is a Hub?
- Which OSI layer does a Hub operate on?
- How does a Hub work?
- What is broadcasting in a Hub?
- What is a collision?

### Intermediate

- Why does a Hub create collisions?
- What is a collision domain?
- Why are hubs considered insecure?
- What is the difference between a Hub and a Repeater?
- Why have switches replaced hubs?

---

# 📌 Key Takeaways

- A Hub is a Layer 1 networking device.
- It broadcasts every incoming frame to all connected devices.
- Hubs do not understand MAC or IP addresses.
- All devices connected to a hub share one collision domain.
- Network collisions reduce overall performance.
- Hubs have been replaced by switches in modern networks.

---

# 📚 References

- Cisco Networking Academy
- CompTIA Network+
- IEEE Ethernet Standards
- Microsoft Learn
