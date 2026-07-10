# Ring Topology
# 📖 Overview

A **Ring Topology** is a network topology in which each device is connected to **two neighboring devices**, forming a circular communication path.

Data travels from one device to the next until it reaches its destination. Since the network forms a closed loop, every device participates in forwarding data.

Ring Topology was widely used in **Token Ring** and **Fiber Distributed Data Interface (FDDI)** networks.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What is Ring Topology?
- How Ring Topology works
- Components of Ring Topology
- Advantages and Disadvantages
- Real-world applications

---

# 📑 Table of Contents

- What is Ring Topology?
- Components
- How Ring Topology Works
- Advantages
- Disadvantages
- Applications
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is Ring Topology?

A **Ring Topology** is a network structure where each device is connected to two other devices, creating a circular path for communication.

Unlike Bus Topology, there is no central communication cable. Instead, every device acts as an intermediate point that forwards data to the next device in the ring.

---

# 🧩 Components of Ring Topology

A Ring Topology typically consists of:

- Computers (Nodes)
- Network Interface Cards (NICs)
- Communication Links (Ethernet/Fiber)
- Network Devices (if required)

Each device has exactly two neighboring connections.

---

# ⚙️ How Ring Topology Works

The communication process is as follows:

1. A device sends data into the ring.
2. The data travels from one device to the next.
3. Each intermediate device forwards the data.
4. The destination device receives the data.
5. The data continues around the ring until transmission is complete.

In many traditional Ring networks, **Token Passing** is used to control communication and prevent data collisions.

---

# 🪙 Token Passing

A **Token** is a small control frame that continuously circulates around the ring.

- A device must possess the token before transmitting data.
- Once the transmission is complete, the token is released for the next device.
- This mechanism prevents multiple devices from transmitting simultaneously.

---

# ✅ Advantages

- No data collisions due to Token Passing.
- Predictable network performance.
- Equal access for all devices.
- Better performance than Bus Topology under heavy network traffic.
- Efficient data transmission.

---

# ❌ Disadvantages

- Failure of a single cable or device may interrupt the entire network.
- Adding or removing devices can temporarily disrupt communication.
- Troubleshooting can be difficult.
- Less scalable than Star Topology.
- Rarely used in modern Ethernet networks.

---

# 🌍 Applications

Ring Topology has been used in:

- Token Ring Networks
- FDDI (Fiber Distributed Data Interface)
- Industrial Control Networks
- Metropolitan Area Networks (MANs)
- Legacy Enterprise Networks

> **Note:** Modern LANs generally prefer **Star Topology** because it offers easier management and better fault tolerance.

---

# 📷 Diagram

Save the diagram as:

```
images/ring-topology.png
```

Recommended diagram:

- Four or five computers connected in a closed circular loop.
- Include arrows indicating the direction of data flow around the ring.

Suggested sources:

- https://commons.wikimedia.org/wiki/Category:Computer_network_diagrams
- https://en.wikipedia.org/wiki/Ring_network

---

# 🎤 Interview Questions

### Beginner

- What is Ring Topology?
- Why is it called Ring Topology?
- What is Token Passing?
- How many neighboring devices is each node connected to?

### Intermediate

- Explain the working of Ring Topology.
- How does Token Passing prevent data collisions?
- What are the advantages and disadvantages of Ring Topology?
- Why is Ring Topology less common in modern LANs?

---

# 📌 Key Takeaways

- Ring Topology connects devices in a circular loop.
- Each device is connected to exactly two neighboring devices.
- Data travels around the ring until it reaches its destination.
- Token Passing is commonly used to prevent data collisions.
- Although reliable for controlled communication, Ring Topology has largely been replaced by Star Topology in modern Ethernet networks.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- IEEE Networking Standards
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
