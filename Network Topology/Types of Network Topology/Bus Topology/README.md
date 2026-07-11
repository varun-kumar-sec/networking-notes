# Bus Topology
# 📖 Overview

A **Bus Topology** is one of the simplest and earliest network topologies in which all devices are connected to a **single central communication cable**, known as the **backbone cable**.

All devices share this common cable to send and receive data. When one device transmits data, the signal travels along the backbone until it reaches the intended destination.

Bus topology was widely used in early Local Area Networks (LANs) because of its simple design and low installation cost.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What is Bus Topology?
- How Bus Topology works
- Components of Bus Topology
- Advantages and Disadvantages
- Real-world applications

---

# 📑 Table of Contents

- What is Bus Topology?
- Components
- How Bus Topology Works
- Advantages
- Disadvantages
- Applications
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is Bus Topology?

A **Bus Topology** is a network topology in which all devices are connected to a **single backbone cable**.

Every device shares the same communication medium to transmit and receive data.

Since all devices use the same cable, only one device should transmit data at a time to avoid communication conflicts.

---

# 🧩 Components of Bus Topology

A Bus Topology consists of the following components:

- Backbone Cable
- Computers (Nodes)
- Network Interface Card (NIC)
- Connectors
- Terminators

> **Note:** Terminators are placed at both ends of the backbone cable to absorb signals and prevent signal reflection.

---

# ⚙️ How Bus Topology Works

The communication process is as follows:

1. A device sends data onto the backbone cable.
2. The data signal travels in both directions along the cable.
3. Every connected device receives the signal.
4. Only the device with the matching destination address accepts the data.
5. Terminators at both ends absorb the signal to prevent it from reflecting back.

---

# ✅ Advantages

- Simple network design.
- Easy to install.
- Requires less cable than many other topologies.
- Cost-effective for small networks.
- Suitable for temporary network setups.

---

# ❌ Disadvantages

- Failure of the backbone cable can bring down the entire network.
- Performance decreases as more devices are added.
- Difficult to troubleshoot cable faults.
- Data collisions can occur when multiple devices transmit simultaneously.
- Limited scalability.

---

# 🌍 Applications

Bus Topology is commonly used in:

- Small Local Area Networks (LANs)
- Temporary laboratory networks
- Educational demonstrations
- Legacy Ethernet networks

> **Note:** Bus Topology is rarely used in modern enterprise networks because more reliable topologies, such as Star Topology, have replaced it.

---

# 📷 Diagram

![Bus-Topology](https://github.com/varun-kumar-sec/networking-notes/blob/main/Network%20Topology/Types%20of%20Network%20Topology/Bus%20Topology/image/Bus-Topology.jpg?raw=true)

---

# 🎤 Interview Questions

### Beginner

- What is Bus Topology?
- What is the purpose of the backbone cable?
- Why are terminators used in Bus Topology?
- What happens if the backbone cable fails?

### Intermediate

- Explain the working of Bus Topology.
- Why are data collisions common in Bus Topology?
- What are the advantages and disadvantages of Bus Topology?
- Why is Bus Topology rarely used in modern networks?

---

# 📌 Key Takeaways

- Bus Topology connects all devices using a single backbone cable.
- Every device shares the same communication medium.
- Terminators prevent signal reflection at both ends of the cable.
- It is inexpensive and easy to install for small networks.
- Failure of the backbone cable affects the entire network.
- Bus Topology has largely been replaced by Star Topology in modern networking.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- IEEE Networking Standards
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
