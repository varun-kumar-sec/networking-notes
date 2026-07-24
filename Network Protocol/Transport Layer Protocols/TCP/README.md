# Transmission Control Protocol (TCP)
# 📖 Overview

The **Transmission Control Protocol (TCP)** is a Transport Layer protocol that provides **reliable, ordered, and error-checked delivery of data** between devices on a network.

TCP establishes a connection before transmitting data, ensuring that all packets arrive correctly and in the proper order.

Because of its reliability, TCP is widely used by applications where data accuracy is more important than transmission speed.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What is TCP?
- Why TCP is used
- How TCP works
- TCP Three-Way Handshake
- Key features of TCP
- Advantages and limitations
- Real-world applications

---

# 📑 Table of Contents

- What is TCP?
- Why is TCP Needed?
- How TCP Works
- TCP Three-Way Handshake
- Features of TCP
- Advantages
- Limitations
- Real-World Applications
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is TCP?

**TCP (Transmission Control Protocol)** is a Transport Layer protocol that ensures reliable communication between two devices.

Before sending data, TCP establishes a connection between the sender and receiver.

During transmission, TCP:

- Numbers data packets.
- Detects transmission errors.
- Retransmits lost packets.
- Delivers packets in the correct order.
- Confirms successful delivery.

---

# ❓ Why is TCP Needed?

TCP is important because it:

- Ensures reliable communication.
- Prevents data loss.
- Maintains packet order.
- Detects transmission errors.
- Supports applications that require accurate data delivery.

---

# ⚙️ How TCP Works

TCP communication generally follows these steps:

1. Establish a connection.
2. Divide data into segments.
3. Number each segment.
4. Transmit the segments.
5. Receive acknowledgments.
6. Retransmit lost segments if necessary.
7. Close the connection after transmission completes.

---

# 🤝 TCP Three-Way Handshake

Before data transmission begins, TCP establishes a connection using the **Three-Way Handshake**.

### Step 1 – SYN

The client sends a **SYN (Synchronize)** packet to request a connection.

↓

### Step 2 – SYN-ACK

The server replies with a **SYN-ACK (Synchronize Acknowledge)** packet.

↓

### Step 3 – ACK

The client sends an **ACK (Acknowledgment)** packet.

After this process, the connection is established and data transfer begins.

---

# ⭐ Features of TCP

TCP provides several important features:

- Connection-oriented communication.
- Reliable data delivery.
- Error detection.
- Flow control.
- Congestion control.
- Ordered packet delivery.
- Packet retransmission.
- Full-duplex communication.

---

# ✅ Advantages

- Reliable communication.
- Error recovery.
- Ordered data delivery.
- Prevents packet loss.
- Suitable for critical applications.

---

# ❌ Limitations

- Higher overhead than UDP.
- Slower due to acknowledgments.
- Requires connection establishment.
- Increased latency compared to connectionless protocols.

---

# 🌍 Real-World Applications

TCP is commonly used by:

- HTTP / HTTPS
- FTP
- SMTP
- POP3
- IMAP
- SSH
- Database applications
- Web browsing
- Email services
- Online banking

---

# 📷 Diagram

Save the diagram as:

```text
images/tcp-three-way-handshake.png
```

Recommended diagram:

```text
Client                      Server

  SYN  -------------------->

       <---------------- SYN + ACK

  ACK  -------------------->

Connection Established
```

Suggested sources:

- https://commons.wikimedia.org/wiki/Category:Transmission_Control_Protocol
- https://en.wikipedia.org/wiki/Transmission_Control_Protocol

---

# 🎤 Interview Questions

### Beginner

- What is TCP?
- Which OSI layer uses TCP?
- Is TCP connection-oriented or connectionless?
- Why is TCP reliable?

### Intermediate

- Explain the TCP Three-Way Handshake.
- What is flow control?
- What is congestion control?
- Why is TCP slower than UDP?
- Name some protocols that use TCP.

---

# 📌 Key Takeaways

- TCP stands for **Transmission Control Protocol**.
- It operates at the **Transport Layer**.
- TCP is **connection-oriented**.
- It guarantees reliable and ordered data delivery.
- TCP establishes communication using the **Three-Way Handshake**.
- Applications such as HTTP, FTP, SMTP, POP3, IMAP, and SSH use TCP.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- RFC 9293 – Transmission Control Protocol (TCP)
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
