# Network Collision
# 📖 Overview

A **network collision** occurs when two or more devices attempt to transmit data over the same shared network medium at the same time.

When this happens, the transmitted signals interfere with one another, causing the data to become corrupted. The devices must then stop transmitting, wait for a random period, and retransmit their data.

Network collisions were common in older Ethernet networks that used **hubs** and operated in **half-duplex** mode. Modern switched Ethernet networks running in **full-duplex** mode have virtually eliminated collisions.

---

# 🎯 Learning Objectives

After completing this topic, you will be able to:

- Understand what a network collision is.
- Explain why collisions occur.
- Identify common symptoms.
- Diagnose collision-related problems.
- Apply appropriate solutions.
- Prevent collisions in modern networks.

---

# 📑 Table of Contents

- What is a Network Collision?
- Why Do Collisions Occur?
- Common Causes
- Symptoms
- How to Identify the Problem
- How to Fix the Problem
- Prevention
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is a Network Collision?

A **network collision** occurs when multiple devices transmit data simultaneously on the same shared communication medium.

Since Ethernet devices cannot process multiple transmissions at exactly the same time on a shared medium, the signals interfere with each other and both transmissions fail.

The devices must retransmit the data after waiting for a random period.

---

# ❓ Why Do Collisions Occur?

Collisions typically occur in networks that:

- Use Ethernet hubs.
- Operate in half-duplex mode.
- Share the same communication medium.
- Have multiple devices transmitting simultaneously.

Modern Ethernet switches isolate communication between devices, greatly reducing the possibility of collisions.

---

# ⚠️ Common Causes

Network collisions are commonly caused by:

- Ethernet hubs
- Half-duplex communication
- High network traffic
- Duplex mismatches
- Multiple devices sharing the same collision domain

---

# 🔍 Symptoms

Common symptoms include:

- Slow network performance
- Frequent retransmissions
- High network latency
- Reduced throughput
- Intermittent communication delays

---

# 🛠️ How to Identify the Problem

### Check Switch or Hub Statistics

Many managed switches report:

- Collision count
- Late collisions
- Frame errors

A high collision count may indicate a problem.

---

### Verify Duplex Settings

Ensure both connected devices use compatible duplex settings.

A duplex mismatch can produce symptoms similar to excessive collisions.

---

### Monitor Network Performance

High latency and poor throughput on a shared Ethernet segment may indicate collisions.

---

# 🔧 How to Fix the Problem

To reduce or eliminate collisions:

1. Replace hubs with switches.
2. Configure devices for full-duplex communication.
3. Verify duplex settings match on both ends of the connection.
4. Reduce unnecessary network traffic.
5. Upgrade outdated network hardware if necessary.

---

# 🛡️ Prevention

Prevent collisions by:

- Using Ethernet switches instead of hubs.
- Configuring full-duplex communication.
- Matching duplex settings on connected devices.
- Monitoring network performance regularly.
- Segmenting large networks when appropriate.

---

# 🎤 Interview Questions

### Beginner

- What is a network collision?
- In which type of network are collisions most common?
- Which device is more likely to cause collisions: a hub or a switch?
- How do devices recover after a collision?

### Intermediate

- Why are collisions rare in modern switched networks?
- Explain the relationship between collisions and half-duplex communication.
- How can a duplex mismatch affect network performance?
- What are collision domains?

---

# 📌 Key Takeaways

- A network collision occurs when two or more devices transmit simultaneously on a shared medium.
- Collisions were common in hub-based Ethernet networks.
- Full-duplex switched Ethernet has largely eliminated collisions.
- Duplex mismatches can produce collision-like symptoms.
- Replacing hubs with switches is the most effective way to prevent collisions.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- IEEE 802.3 Ethernet Standards
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
