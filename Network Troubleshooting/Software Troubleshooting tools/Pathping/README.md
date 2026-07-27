# PathPing
# 📖 Overview

**PathPing** is a Windows command-line network diagnostic tool that combines the functionality of **Ping** and **Tracert**.

Like **Tracert**, it discovers the route that packets take to reach a destination. Like **Ping**, it measures packet loss and latency. However, instead of testing only the destination, PathPing analyzes **every router (hop)** along the path.

This makes it especially useful for identifying where packet loss or network congestion occurs.

---

# 🎯 Learning Objectives

After completing this topic, you will be able to:

- Understand what PathPing is.
- Explain how PathPing works.
- Interpret PathPing results.
- Identify packet loss in a network path.
- Recognize the advantages and limitations of PathPing.

---

# 📑 Table of Contents

- What is PathPing?
- How PathPing Works
- Why PathPing is Used
- Understanding PathPing Output
- Common Troubleshooting Scenarios
- Limitations
- Example
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is PathPing?

**PathPing** is a network diagnostic utility available in Microsoft Windows.

It first traces the route to a destination and then sends multiple ICMP packets to every router along that path.

This allows PathPing to identify:

- Packet loss
- High latency
- Network congestion
- Problematic routers

Unlike Ping, PathPing analyzes the **entire communication path**, not just the destination.

---

# ⚙️ How PathPing Works

PathPing performs two stages:

### Stage 1 – Route Discovery

It identifies every router between the source and destination, similar to Tracert.

### Stage 2 – Performance Analysis

It sends multiple ICMP Echo Requests to every hop.

After collecting statistics, it reports:

- Packet loss
- Round-trip time
- Network performance for each hop

Because of this analysis, PathPing takes longer to complete than Ping or Tracert.

---

# 🎯 Why PathPing is Used

Network administrators use PathPing to:

- Locate packet loss.
- Identify congested routers.
- Troubleshoot intermittent network problems.
- Verify network reliability.
- Analyze end-to-end network performance.

---

# 📊 Understanding PathPing Output

A typical report includes:

- Hop number
- Router IP address
- Latency
- Packet loss percentage

Example:

```text
Hop  RTT   Lost/Sent = Pct

1    <1ms   0/100 = 0%
2     8ms   0/100 = 0%
3    24ms  12/100 = 12%
4    28ms   0/100 = 0%
```

In this example:

- Hop 3 is experiencing packet loss.
- The network administrator should investigate that router or its connection.

---

# 🔍 Common Troubleshooting Scenarios

### Packet Loss at One Hop

Possible causes:

- Congested router
- Faulty interface
- Damaged cable
- Hardware failure

---

### High Latency

May indicate:

- Heavy network traffic
- Long-distance routing
- Busy routers

---

### Packet Loss Across Multiple Hops

Possible causes:

- WAN problems
- ISP issues
- Network congestion
- Physical layer faults

---

### No Packet Loss

Indicates that the network path is operating normally.

---

# ⚠️ Limitations

PathPing has several limitations:

- Takes longer to complete than Ping or Tracert.
- Uses ICMP, which some routers or firewalls block.
- High latency on one hop does not always indicate a problem.
- Available only on Microsoft Windows.

---

# 💻 Example

### Windows

```cmd
pathping google.com
```

Example output:

```text
Tracing route...

Computing statistics...

Hop  RTT   Lost/Sent = Pct

1    <1ms   0/100 = 0%
2     9ms   0/100 = 0%
3    23ms   8/100 = 8%
4    27ms   0/100 = 0%
```

---

# 📷 Diagram

![Pathping](https://github.com/varun-kumar-sec/networking-notes/blob/main/Network%20Troubleshooting/Image/Pathping.png?raw=true)

---

# 🎤 Interview Questions

### Beginner

- What is PathPing?
- How is PathPing different from Ping?
- What information does PathPing provide?
- Why does PathPing take longer to complete?

### Intermediate

- Explain how PathPing combines Ping and Tracert.
- What does packet loss indicate?
- How can PathPing help locate network congestion?
- Why might PathPing report packet loss at a specific router?

---

# 📌 Key Takeaways

- PathPing combines the functionality of Ping and Tracert.
- It analyzes every router between the source and destination.
- It measures packet loss and latency for each hop.
- It is useful for diagnosing network congestion and unreliable connections.
- PathPing is one of the most powerful built-in Windows network troubleshooting tools.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- Microsoft Learn – PathPing Command
- RFC 791 – Internet Protocol
- RFC 792 – Internet Control Message Protocol
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
