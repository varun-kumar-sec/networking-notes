# Traceroute Command (tracert / traceroute)
# 📖 Overview

The **Traceroute** command is a network diagnostic tool used to determine the path that data packets take from a source device to a destination device.

Unlike the **ping** command, which only verifies whether a destination is reachable, traceroute displays every router (hop) the packet passes through along its journey.

This makes traceroute an essential tool for identifying routing issues, network delays, and points of failure.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What is traceroute?
- Why traceroute is used
- How traceroute works
- Basic traceroute syntax
- Understanding hops
- Common traceroute commands
- Real-world applications

---

# 📑 Table of Contents

- What is Traceroute?
- Why Use Traceroute?
- How Traceroute Works
- Basic Syntax
- Understanding Hops
- Common Commands
- Real-World Applications
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is Traceroute?

Traceroute is a command-line utility that displays the path taken by packets from the source device to the destination.

Each router that forwards the packet is displayed as a **hop**.

This allows network administrators to identify where communication problems occur.

---

# ❓ Why Use Traceroute?

Traceroute helps users:

- View the path to a destination.
- Identify routing problems.
- Detect slow network links.
- Locate failed routers.
- Troubleshoot Internet connectivity.

---

# ⚙️ How Traceroute Works

Traceroute works by sending packets with gradually increasing **Time To Live (TTL)** values.

The process is:

1. Send a packet with **TTL = 1**.
2. The first router decreases the TTL to 0 and returns an ICMP Time Exceeded message.
3. Send another packet with **TTL = 2**.
4. The second router responds.
5. This process continues until the destination is reached.

Each responding router represents one **hop**.

---

# 💻 Basic Syntax

## Windows

```cmd
tracert <destination>
```

Example:

```cmd
tracert google.com
```

---

## Linux / macOS

```bash
traceroute <destination>
```

Example:

```bash
traceroute google.com
```

---

# 📋 Example Output

```text
Tracing route to google.com

1   1 ms    1 ms    1 ms    192.168.1.1
2   9 ms   10 ms    8 ms    ISP Router
3  18 ms   19 ms   20 ms    Core Router
4  25 ms   24 ms   26 ms    google.com
```

This output shows:

- Hop 1 → Home router
- Hop 2 → ISP router
- Hop 3 → Intermediate router
- Hop 4 → Destination server

---

# 📍 Understanding Hops

A **hop** is any networking device (usually a router) that forwards a packet toward its destination.

For example:

```text
Computer

↓

Router 1

↓

Router 2

↓

Router 3

↓

Destination
```

This path contains **4 hops**.

---

# 🌍 Real-World Applications

Traceroute is commonly used to:

- Diagnose routing problems.
- Identify slow network paths.
- Locate failed routers.
- Troubleshoot Internet connectivity.
- Verify the route to a remote server.

---

# 📷 Diagram

![Traceroute](https://github.com/varun-kumar-sec/networking-notes/blob/main/IP%20Addressing/Image/Traceroute.png?raw=true)

---

# 🎤 Interview Questions

### Beginner

- What is traceroute?
- What is a hop?
- Which Windows command performs traceroute?
- Which Linux command performs traceroute?

### Intermediate

- Explain how traceroute works.
- What is the purpose of the TTL field?
- Why might traceroute stop before reaching the destination?
- What is the difference between ping and traceroute?

---

# 📌 Key Takeaways

- Traceroute displays the path packets take to reach a destination.
- Windows uses the **tracert** command.
- Linux and macOS use the **traceroute** command.
- Each router along the path is called a **hop**.
- Traceroute uses increasing **TTL values** to discover each hop.
- It is commonly used to troubleshoot routing and connectivity issues.

---

# 📚 References

- Microsoft Learn – tracert Command
- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- RFC 791 – Internet Protocol (IPv4)
