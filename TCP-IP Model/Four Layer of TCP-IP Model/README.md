# Four Layers of the TCP/IP Model
# 📖 Overview

The **TCP/IP (Transmission Control Protocol/Internet Protocol) Model** divides network communication into **four layers**, where each layer performs a specific networking function.

Unlike the OSI Model, the TCP/IP Model is a **practical networking model** that is implemented in modern operating systems, networking devices, and Internet protocols.

Each layer provides services to the layer above it while using the services of the layer below it. Together, these layers enable reliable communication across local and global networks.

---

# 🎯 Learning Objectives

After completing this section, you will be able to:

- Identify all four layers of the TCP/IP Model.
- Understand the responsibilities of each layer.
- Recognize the Protocol Data Unit (PDU) used by each layer.
- Identify common protocols and devices associated with each layer.
- Understand how data moves through the TCP/IP protocol stack.

---

# 📂 Directory Structure

```text
Four Layers of TCP/IP Model
│
├── Application Layer
├── Transport Layer
├── Internet Layer
└── Network Access Layer
```

---

# 📚 The Four Layers

| Layer | Name | Primary Responsibility |
|------:|------|------------------------|
| 4 | Application Layer | Provides network services to user applications |
| 3 | Transport Layer | End-to-end communication and reliable data delivery |
| 2 | Internet Layer | Logical addressing and routing |
| 1 | Network Access Layer | Framing, MAC addressing, and physical transmission |

---

# 📦 Protocol Data Units (PDUs)

Each TCP/IP layer uses a specific Protocol Data Unit (PDU).

| Layer | PDU |
|------:|-----|
| Application | Data |
| Transport | Segment |
| Internet | Packet |
| Network Access | Frame → Bits |

---

# 🖥️ Common Devices

Different networking devices primarily operate at different TCP/IP layers.

| Layer | Common Device |
|------:|---------------|
| Application | Computer, Server |
| Transport | Firewall (some functions) |
| Internet | Router, Layer 3 Switch |
| Network Access | Switch, NIC, Hub, Bridge, Repeater, Wireless Access Point |

---

# 🌐 Common Protocols

| Layer | Example Protocols |
|------:|-------------------|
| Application | HTTP, HTTPS, FTP, DNS, DHCP, SMTP, IMAP, POP3, SSH |
| Transport | TCP, UDP |
| Internet | IPv4, IPv6, ICMP, IGMP |
| Network Access | Ethernet (IEEE 802.3), Wi-Fi (IEEE 802.11), PPP |

---

# 🔄 Data Flow Through the TCP/IP Model

During transmission, data moves from the top layer to the bottom layer.

```text
Application
      ↓
Transport
      ↓
Internet
      ↓
Network Access
```

At the receiving device, the process is reversed.

```text
Network Access
      ↑
Internet
      ↑
Transport
      ↑
Application
```

This process is known as **Encapsulation** and **Decapsulation**.

---

# 💡 Memory Trick

A simple way to remember the TCP/IP layers from **top to bottom** is:

> **Applications Travel Into Networks**

| Word | Layer |
|------|-------|
| Applications | Application Layer |
| Travel | Transport Layer |
| Into | Internet Layer |
| Networks | Network Access Layer |

---

# 🌍 Why Are the Layers Important?

The layered architecture provides several benefits:

- Simplifies network communication.
- Makes troubleshooting easier.
- Supports interoperability between different systems.
- Allows protocols to evolve independently.
- Enables scalable Internet communication.


---

# 📌 Key Takeaways

- The TCP/IP Model consists of **four layers**.
- It is the networking model used by the Internet.
- Each layer has a specific responsibility.
- Every layer uses its own Protocol Data Unit (PDU).
- Data moves downward during encapsulation and upward during decapsulation.
- The TCP/IP Model provides the foundation for modern network communication.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- RFC 791 – Internet Protocol (IPv4)
- RFC 793 – Transmission Control Protocol (TCP)
- RFC 8200 – Internet Protocol Version 6 (IPv6)
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
