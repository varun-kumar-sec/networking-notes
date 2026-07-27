# Tracert
# 📖 Overview

**Tracert** (Windows) or **Traceroute** (Linux/macOS) is a network troubleshooting tool used to discover the path that packets take from a source device to a destination.

Unlike **Ping**, which only tells you whether a destination is reachable, **Tracert** identifies every router (hop) along the route and measures the time taken to reach each one.

It helps network administrators locate where communication problems occur within a network.

---

# 🎯 Learning Objectives

After completing this topic, you will be able to:

- Understand Tracert as a troubleshooting tool.
- Explain how Tracert works.
- Interpret Tracert output.
- Identify routing problems.
- Understand the limitations of Tracert.

---

# 📑 Table of Contents

- What is Tracert?
- How Tracert Works
- Why Tracert is Used
- Understanding Tracert Output
- Common Troubleshooting Scenarios
- Limitations
- Example
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is Tracert?

**Tracert** is a command-line utility that displays the sequence of routers (called **hops**) that packets pass through before reaching their destination.

It helps answer questions such as:

- Where is the network delay occurring?
- Which router is unreachable?
- Is the routing path correct?

---

# ⚙️ How Tracert Works

Tracert works by sending packets with increasing **Time To Live (TTL)** values.

The process is:

1. Send a packet with **TTL = 1**.
2. The first router decreases TTL to 0 and returns an ICMP Time Exceeded message.
3. Tracert records that router.
4. The next packet is sent with **TTL = 2**.
5. The process repeats until the destination is reached.

This gradually reveals every router along the path.

---

# 🎯 Why Tracert is Used

Network administrators use Tracert to:

- Identify routing problems.
- Locate network delays.
- Discover where packets are being dropped.
- Verify the routing path.
- Troubleshoot connectivity issues beyond the local network.

---

# 📊 Understanding Tracert Output

A typical Tracert result includes:

- Hop number
- Router IP address or hostname
- Response time for each hop

Example:

```text
1   <1 ms    <1 ms    <1 ms    192.168.1.1
2    8 ms     9 ms     8 ms    10.20.30.1
3   14 ms    15 ms    14 ms    203.0.113.1
4   18 ms    17 ms    18 ms    8.8.8.8
```

Each numbered line represents one router between the source and destination.

---

# 🔍 Common Troubleshooting Scenarios

### High Response Time

May indicate:

- Network congestion
- Busy router
- Long-distance routing

---

### Request Timed Out (* * *)

May indicate:

- Router blocking ICMP
- Firewall restrictions
- Router configured not to reply
- Temporary network congestion

A timeout at one hop does **not always** indicate a network failure.

---

### Traceroute Stops Before Destination

Possible causes include:

- Routing failure
- Network outage
- Firewall blocking packets
- Destination network unavailable

---

### Unexpected Routing Path

May indicate:

- Incorrect routing configuration
- ISP routing changes
- Routing loops
- Misconfigured routers

---

# ⚠️ Limitations

Tracert has several limitations:

- Some routers intentionally block ICMP.
- Timeouts do not always indicate a fault.
- High latency at one hop may not affect later hops.
- Tracert cannot diagnose application-layer problems.

---

# 💻 Example

### Windows

```cmd
tracert google.com
```

### Linux/macOS

```bash
traceroute google.com
```

Example output:

```text
Tracing route to google.com

1   <1 ms    192.168.1.1
2    9 ms    ISP Router
3   16 ms    Regional Router
4   22 ms    google.com
```

---

# 📷 Diagram

![Tracert](https://github.com/varun-kumar-sec/networking-notes/blob/main/Network%20Troubleshooting/Image/tracert.jpg?raw=true)

---

# 🎤 Interview Questions

### Beginner

- What is Tracert?
- What information does Tracert provide?
- What is a hop?
- What does Tracert use the TTL field for?

### Intermediate

- Explain how Tracert discovers each router along the path.
- Why might a router display "* * *" during a trace?
- What is the difference between Ping and Tracert?
- How does Tracert help identify routing problems?

---

# 📌 Key Takeaways

- Tracert identifies every router between the source and destination.
- It uses increasing TTL values to discover each hop.
- It helps diagnose routing problems and network delays.
- A timeout at a single hop does not always indicate a failure.
- Tracert complements Ping by showing **where** communication problems occur.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- Microsoft Learn – Tracert Command
- RFC 791 – Internet Protocol
- RFC 792 – Internet Control Message Protocol
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
