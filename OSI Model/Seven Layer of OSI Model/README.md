# Seven Layers of the OSI Model
# 📖 Overview

The **OSI (Open Systems Interconnection) Model** divides network communication into **seven layers**, where each layer performs a specific function.

Each layer communicates only with the layer directly above and below it. This layered architecture simplifies network design, protocol development, troubleshooting, and communication between different networking devices.

Together, these seven layers define how data travels from one device to another across a network.

---

# 🎯 Learning Objectives

After completing this section, you will be able to:

- Identify all seven layers of the OSI Model.
- Understand the primary responsibility of each layer.
- Recognize the Protocol Data Unit (PDU) used by each layer.
- Identify common devices and protocols associated with each layer.
- Understand how the layers work together during communication.

---

# 📂 Directory Structure

```text
Seven Layers of OSI Model
│
├── Physical Layer
├── Data Link Layer
├── Network Layer
├── Transport Layer
├── Session Layer
├── Presentation Layer
└── Application Layer
```

---

# 📚 The Seven Layers

| Layer | Name | Primary Responsibility |
|------:|------|------------------------|
| 7 | Application Layer | Provides network services to end-user applications |
| 6 | Presentation Layer | Translation, encryption, and compression |
| 5 | Session Layer | Establishes, manages, and terminates communication sessions |
| 4 | Transport Layer | End-to-end communication and reliable data delivery |
| 3 | Network Layer | Routing and logical addressing |
| 2 | Data Link Layer | Framing, MAC addressing, and error detection |
| 1 | Physical Layer | Transmission of raw bits over the communication medium |

---

# 📦 Protocol Data Units (PDUs)

Each layer uses a specific Protocol Data Unit (PDU).

| Layer | PDU |
|------:|-----|
| Application | Data |
| Presentation | Data |
| Session | Data |
| Transport | Segment |
| Network | Packet |
| Data Link | Frame |
| Physical | Bits |

---

# 🖥️ Common Devices

Different networking devices operate at different OSI layers.

| Layer | Common Device |
|------:|---------------|
| Application | Application Software |
| Presentation | — |
| Session | — |
| Transport | Firewall (some functions) |
| Network | Router, Layer 3 Switch |
| Data Link | Switch, Bridge |
| Physical | Hub, Repeater, Cables |

---

# 🌐 Common Protocols

| Layer | Example Protocols |
|------:|-------------------|
| Application | HTTP, HTTPS, FTP, SMTP, DNS, DHCP |
| Presentation | SSL/TLS, ASCII, Unicode, JPEG, PNG |
| Session | RPC, NetBIOS |
| Transport | TCP, UDP |
| Network | IPv4, IPv6, ICMP, IGMP |
| Data Link | Ethernet (IEEE 802.3), Wi-Fi (IEEE 802.11), PPP |
| Physical | IEEE 802 Standards, Ethernet Physical Signaling |

---

# 🔄 Data Flow Through the OSI Model

During transmission, data moves **from the Application Layer to the Physical Layer**.

```text
Application
      ↓
Presentation
      ↓
Session
      ↓
Transport
      ↓
Network
      ↓
Data Link
      ↓
Physical
```

At the receiving device, the process is reversed:

```text
Physical
      ↑
Data Link
      ↑
Network
      ↑
Transport
      ↑
Session
      ↑
Presentation
      ↑
Application
```

This process is known as **Encapsulation** and **Decapsulation**.

---

# 💡 Memory Trick

A popular mnemonic to remember the layers from **Layer 7 to Layer 1** is:

> **All People Seem To Need Data Processing**

| Mnemonic | Layer |
|-----------|-------|
| All | Application |
| People | Presentation |
| Seem | Session |
| To | Transport |
| Need | Network |
| Data | Data Link |
| Processing | Physical |

---

# 🌍 Why Are the Layers Important?

The layered architecture provides several benefits:

- Simplifies network communication.
- Makes troubleshooting easier.
- Encourages standardization.
- Supports interoperability between vendors.
- Allows independent development of networking protocols.


---

# 📌 Key Takeaways

- The OSI Model consists of **seven layers**.
- Each layer performs a specific networking function.
- Every layer has its own Protocol Data Unit (PDU).
- Different networking devices operate at different layers.
- Data moves downward during encapsulation and upward during decapsulation.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- ISO/IEC 7498-1 (OSI Reference Model)
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
