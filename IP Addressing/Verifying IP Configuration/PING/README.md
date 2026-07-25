# Ping Command
# 📖 Overview

The **ping** command is one of the most commonly used network troubleshooting tools. It is used to verify whether a device can communicate with another device over an IP network.

The command works by sending **ICMP (Internet Control Message Protocol) Echo Request** messages to a destination device and waiting for **ICMP Echo Reply** messages.

If replies are received, the destination is reachable. If no replies are received, there may be a connectivity problem.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What is the ping command?
- Why ping is used
- How ping works
- Basic ping syntax
- Common ping options
- Interpreting ping results
- Real-world applications

---

# 📑 Table of Contents

- What is Ping?
- Why Use Ping?
- How Ping Works
- Basic Syntax
- Common Commands
- Understanding Ping Results
- Real-World Applications
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🖥️ What is Ping?

**Ping** is a command-line utility used to test connectivity between two devices on an IP network.

It measures:

- Whether the destination is reachable
- Round-trip time (RTT)
- Packet loss

---

# ❓ Why Use Ping?

Ping helps users:

- Verify network connectivity
- Test communication with another device
- Check Internet connectivity
- Troubleshoot network problems
- Measure network latency

---

# ⚙️ How Ping Works

The process is as follows:

1. The source device sends an **ICMP Echo Request** packet.
2. The destination device receives the request.
3. If reachable, it sends an **ICMP Echo Reply**.
4. The source measures the time taken for the reply.

If no reply is received within the timeout period, the request is considered unsuccessful.

---

# 💻 Basic Syntax

## Windows

```cmd
ping <destination>
```

Example:

```cmd
ping google.com
```

or

```cmd
ping 8.8.8.8
```

---

## Linux / macOS

```bash
ping <destination>
```

Example:

```bash
ping google.com
```

---

# 📋 Common Ping Commands

## Ping an IP Address

```cmd
ping 192.168.1.1
```

---

## Ping a Domain Name

```cmd
ping google.com
```

---

## Send Four Requests (Windows Default)

```cmd
ping google.com
```

Windows sends **4 Echo Requests** by default.

---

## Send Continuous Requests (Windows)

```cmd
ping -t google.com
```

Stops with:

```text
Ctrl + C
```

---

## Specify Number of Requests (Linux/macOS)

```bash
ping -c 4 google.com
```

---

# 📊 Understanding Ping Results

### Successful Ping

```text
Reply from 192.168.1.1:
bytes=32
time=5ms
TTL=64
```

This indicates:

- Destination reachable
- Packet successfully returned

---

### Request Timed Out

```text
Request timed out.
```

Possible causes:

- Destination offline
- Firewall blocking ICMP
- Network failure

---

### Destination Host Unreachable

```text
Destination host unreachable.
```

Possible causes:

- Incorrect IP configuration
- Router problem
- Network disconnected

---

# 🌍 Real-World Applications

Ping is commonly used to:

- Test Internet connectivity
- Verify local network communication
- Check server availability
- Measure network latency
- Troubleshoot connectivity issues

---

# 📷 Diagram

![Ping](https://github.com/varun-kumar-sec/networking-notes/blob/main/IP%20Addressing/Image/ping.png?raw=true)

---

# 🎤 Interview Questions

### Beginner

- What is the ping command?
- What protocol does ping use?
- What does ping test?
- What is round-trip time (RTT)?

### Intermediate

- Explain how ping works.
- What does "Request timed out" mean?
- What does "Destination host unreachable" mean?
- Why might a server not respond to ping even though it is online?

---

# 📌 Key Takeaways

- **Ping** is a network troubleshooting utility.
- It uses **ICMP Echo Request** and **Echo Reply** messages.
- It verifies whether a destination device is reachable.
- It measures **latency (RTT)** and **packet loss**.
- Ping is one of the first commands used when diagnosing network connectivity problems.

---

# 📚 References

- Microsoft Learn – Ping Command
- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- RFC 792 – Internet Control Message Protocol (ICMP)
