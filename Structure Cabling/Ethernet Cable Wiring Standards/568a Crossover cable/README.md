# T568A Wiring Standard (Used in Crossover Cables)
# 📖 Overview

**T568A** is one of the two standard wiring schemes defined by the **TIA/EIA-568** standard for terminating Ethernet cables.

It specifies the order in which the eight wires inside a twisted pair cable are arranged before being inserted into an **RJ45 connector**.

When one end of an Ethernet cable is wired using **T568A** and the other end is wired using **T568B**, the cable becomes a **Crossover Cable**.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What is T568A?
- Why T568A is used
- Wire color sequence
- What is a crossover cable?
- Applications of crossover cables

---

# 📑 Table of Contents

- What is T568A?
- Wire Color Sequence
- What is a Crossover Cable?
- Applications
- Advantages
- Interview Questions
- Key Takeaways
- References

---

# 🔧 What is T568A?

**T568A** is a standardized wiring arrangement used when terminating Ethernet cables with **RJ45 connectors**.

It defines the exact order of the eight conductors inside a twisted pair cable.

Following this standard ensures proper communication between networking devices.

---

# 🌈 T568A Wire Color Sequence

The wire sequence for **T568A** is:

| Pin | Wire Color |
|-----:|------------|
| 1 | White/Green |
| 2 | Green |
| 3 | White/Orange |
| 4 | Blue |
| 5 | White/Blue |
| 6 | Orange |
| 7 | White/Brown |
| 8 | Brown |

---

# 🔄 What is a Crossover Cable?

A **Crossover Cable** is created by terminating:

- One end using **T568A**
- The other end using **T568B**

This swaps the transmit (TX) and receive (RX) wire pairs, allowing similar networking devices to communicate directly.

Example:

```
End A → T568A
End B → T568B
```

---

# 🌍 Applications

Crossover cables are traditionally used to connect similar devices directly, such as:

- Computer ↔ Computer
- Switch ↔ Switch
- Hub ↔ Hub
- Router ↔ Router

> **Note:** Most modern networking devices support **Auto MDI-X**, so crossover cables are less commonly required today.

---

# ✅ Advantages

- Standardized wiring arrangement
- Reliable Ethernet communication
- Required for creating crossover cables
- Easy identification of wire sequence

---

# 📷 Diagram

![568a-Wiring](https://github.com/varun-kumar-sec/networking-notes/blob/main/Structure%20Cabling/Ethernet%20Cable%20Wiring%20Standards/568a%20Crossover%20cable/image/T568A-Wiring.jpg?raw=true)

---

# 🎤 Interview Questions

### Beginner

- What is T568A?
- Is T568A a wiring standard or a cable type?
- What is the wire color sequence of T568A?
- When is T568A used?

### Intermediate

- How is a crossover cable created?
- What is the difference between T568A and T568B?
- Why is T568A used in crossover cables?
- Why are crossover cables less common today?

---

# 📌 Key Takeaways

- T568A is an Ethernet wiring standard defined by TIA/EIA-568.
- It specifies the wire order inside an RJ45 connector.
- A crossover cable is created by using T568A on one end and T568B on the other.
- Crossover cables are used to connect similar networking devices directly.
- Modern devices often eliminate the need for crossover cables through Auto MDI-X.

---

# 📚 References

- Cisco Networking Academy
- CompTIA Network+
- TIA/EIA-568 Standard
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
