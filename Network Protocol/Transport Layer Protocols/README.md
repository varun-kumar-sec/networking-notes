# 🚚 Transport Layer Protocols

The **Transport Layer** is responsible for providing end-to-end communication between applications running on different devices. It ensures that data is delivered to the correct application and manages how data is transmitted across the network.

Transport Layer protocols determine whether communication should prioritize **reliability** or **speed**. Some applications require guaranteed data delivery, while others prioritize low latency and can tolerate occasional packet loss.

This directory covers the two primary Transport Layer protocols used in modern networks:

- **TCP (Transmission Control Protocol)** – Reliable, connection-oriented communication.
- **UDP (User Datagram Protocol)** – Fast, connectionless communication.

Understanding these protocols is essential because many higher-layer protocols rely on either TCP or UDP for data transmission.

---

## 📂 Directory Structure

```text
04-transport-layer-protocols/
├── TCP/
└── UDP/
```

---

## 📚 Topics Covered

### 🔹 TCP (Transmission Control Protocol)

Learn about:

- Connection-oriented communication
- Reliable data delivery
- Three-Way Handshake
- Flow control
- Congestion control
- Error detection and retransmission
- Real-world applications

---

### 🔹 UDP (User Datagram Protocol)

Learn about:

- Connectionless communication
- Datagram transmission
- Low latency communication
- Fast data transfer
- Real-time applications
- Real-world use cases

---

## 🎯 Learning Objectives

After completing this directory, you will be able to:

- Understand the purpose of the Transport Layer.
- Explain the differences between TCP and UDP.
- Understand connection-oriented and connectionless communication.
- Identify applications that use TCP or UDP.
- Explain how reliable communication is achieved using TCP.
- Understand why UDP is preferred for real-time applications.

---

## 📖 Prerequisites

Before studying this directory, you should understand:

- OSI Model
- TCP/IP Model
- What is a Network Protocol?
- What is a Port?

---

## 🎓 Recommended Study Order

1. TCP
2. UDP

---

## 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- RFC 9293 – Transmission Control Protocol (TCP)
- RFC 768 – User Datagram Protocol (UDP)
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
