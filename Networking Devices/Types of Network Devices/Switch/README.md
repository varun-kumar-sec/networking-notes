# Switch
# 📖 Overview

A **Switch** is a Layer 2 (Data Link Layer) networking device that connects multiple devices within a Local Area Network (LAN) and forwards data intelligently using **MAC addresses**.

Unlike a Hub, which broadcasts data to every connected device, a Switch sends data only to the intended destination device. This significantly improves network performance, reduces unnecessary traffic, and eliminates collisions during normal operation.

A Switch is often described as a **multi-port Bridge** because it performs the same intelligent forwarding function but supports many more ports and higher performance.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What a Switch is
- Why a Switch is required
- How a Switch works
- Why a Switch is called an Intelligent Device
- MAC Address Table (CAM Table)
- Collision Domain
- Broadcast Domain
- OSI Layer
- Advantages and disadvantages
- Security considerations

---

# 📑 Table of Contents

- What is a Switch?
- Why is a Switch Required?
- How Does a Switch Work?
- Why is a Switch called an Intelligent Device?
- MAC Address Table (CAM Table)
- Collision Domain
- Broadcast Domain
- Full Duplex Communication
- OSI Layer
- Advantages
- Disadvantages
- Hub vs Switch
- Real-world Applications
- Security Perspective
- Interview Questions
- Key Takeaways
- References

---

# 🔀 What is a Switch?

A **Switch** is a networking device that connects multiple devices within the same Local Area Network (LAN).

Instead of sending every frame to every connected device, the switch forwards frames only to the destination device using the destination MAC Address.

This makes communication faster, more secure, and more efficient.

---

# ❓ Why is a Switch Required?

A Switch is required to:

- Connect multiple devices within a LAN
- Reduce unnecessary network traffic
- Eliminate collisions
- Improve communication speed
- Increase overall network performance

Modern enterprise networks rely heavily on switches because of their efficiency and scalability.

---

# ⚙️ How Does a Switch Work?

The working process of a switch is as follows:

1. A device sends an Ethernet frame to the switch.
2. The switch reads the **Source MAC Address** and stores it in its MAC Address Table.
3. The switch checks the **Destination MAC Address**.
4. If the destination MAC Address exists in the table, the frame is forwarded only to that specific port.
5. If the destination MAC Address is unknown, the switch temporarily broadcasts the frame.
6. Once the destination responds, its MAC Address is learned and stored for future communication.

This process allows the switch to forward traffic efficiently.

---

# 🧠 Why is a Switch Called an Intelligent Device?

A Switch is considered an **Intelligent Device** because it:

- Learns MAC Addresses automatically
- Maintains a MAC Address Table
- Makes forwarding decisions
- Sends data only to the intended destination
- Reduces unnecessary traffic
- Minimizes collisions

Unlike a Hub, a Switch does not blindly broadcast every frame.

---

# 📋 MAC Address Table (CAM Table)

The Switch maintains a **MAC Address Table**, also known as the **CAM (Content Addressable Memory) Table**.

Example:

| MAC Address | Port |
|-------------|------|
| AA:BB:CC:11:22:33 | Port 1 |
| DD:EE:FF:44:55:66 | Port 2 |
| 11:22:33:44:55:66 | Port 3 |

Whenever a frame arrives, the switch updates this table automatically.

This allows future frames to be forwarded directly to the correct destination.

---

# 💥 Collision Domain

Each switch port creates its **own Collision Domain**.

Example:

```
PC1 ─┐
PC2 ─┤
PC3 ─┤── Switch
PC4 ─┘
```

Each device communicates independently.

As a result:

- Collisions are eliminated during normal operation.
- Network performance improves significantly.

---

# 📡 Broadcast Domain

A Layer 2 Switch **does not separate Broadcast Domains**.

Broadcast traffic is still forwarded to all devices within the same VLAN.

Therefore:

- Collision Domains → Separate ✅
- Broadcast Domain → Shared ❌

> **Note:** VLANs can be used to create separate broadcast domains on managed switches.

---

# 🔄 Full Duplex Communication

Modern switches support **Full Duplex Communication**.

This means:

- Devices can send and receive data simultaneously.
- No collisions occur during normal communication.
- Network throughput increases significantly.

---

# 📡 OSI Layer

A traditional Ethernet Switch operates at:

## **Layer 2 – Data Link Layer**

At this layer, it understands:

- Ethernet Frames
- MAC Addresses

Some advanced switches (Layer 3 Switches) can also perform routing functions.

---

# 🆚 Hub vs Switch

| Feature | Hub | Switch |
|----------|------|---------|
| OSI Layer | Layer 1 | Layer 2 |
| Uses MAC Address | ❌ No | ✅ Yes |
| Intelligent Device | ❌ No | ✅ Yes |
| Collision Domain | One | One per Port |
| Broadcast Traffic | Always | Only when destination is unknown |
| Performance | Low | High |
| Security | Poor | Better |

---

# 🌍 Real-World Applications

Switches are widely used in:

- Enterprise Networks
- Data Centers
- Schools and Universities
- Offices
- Banks
- Cloud Infrastructure
- Campus Networks

Almost every modern LAN uses switches instead of hubs.

---

# ✅ Advantages

- High-speed communication
- Intelligent forwarding
- Eliminates collisions
- Better security than hubs
- Efficient bandwidth utilization
- Supports Full Duplex communication
- Highly scalable

---

# ❌ Disadvantages

- More expensive than hubs
- Managed switches require configuration
- Broadcast traffic still exists without VLANs
- Vulnerable to MAC flooding attacks

---

# 🛡 Security Perspective

Although switches improve security compared to hubs, they are still vulnerable to attacks such as:

- MAC Flooding
- ARP Spoofing
- VLAN Hopping (managed switches)
- CAM Table Overflow

Security features such as:

- Port Security
- VLANs
- DHCP Snooping
- Dynamic ARP Inspection (DAI)

are commonly used to secure modern switches.

---

# 📷 Diagram

![Switch](https://github.com/varun-kumar-sec/networking-notes/blob/main/Networking%20Devices/Types%20of%20Network%20Devices/Switch/image/Switch.png?raw=true)

---

# 🎤 Interview Questions

### Beginner

- What is a Switch?
- Why is a Switch called an Intelligent Device?
- Which OSI layer does a Switch operate on?
- What is a MAC Address Table?
- How does a Switch forward frames?

### Intermediate

- What is the difference between a Hub and a Switch?
- What is a CAM Table?
- Does a Switch reduce collisions?
- Does a Switch reduce broadcast domains?
- What happens if the destination MAC Address is unknown?

---

# 📌 Key Takeaways

- A Switch is a Layer 2 networking device.
- It forwards frames using MAC Addresses.
- Switches maintain a MAC Address (CAM) Table.
- Each switch port creates a separate Collision Domain.
- Broadcast Domains remain shared unless VLANs are configured.
- Switches are intelligent devices because they learn and make forwarding decisions.
- Modern LANs use switches instead of hubs due to their higher performance and security.

---

# 📚 References

- Cisco Networking Academy
- CompTIA Network+
- IEEE 802.3 Ethernet Standard
- Microsoft Learn
