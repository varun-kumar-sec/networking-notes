# TCP/IP Transport Layer
# 📖 Overview

The **Transport Layer** is the **third layer** of the TCP/IP Model. It is responsible for providing **end-to-end communication** between applications running on different devices.

It ensures that data reaches the correct application by using **port numbers**. The Transport Layer also performs **segmentation**, **flow control**, **error detection**, and **reliable data delivery**.

The two primary protocols used at this layer are:

- **TCP (Transmission Control Protocol)**
- **UDP (User Datagram Protocol)**

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What is the TCP/IP Transport Layer?
- Functions of the Transport Layer
- TCP and UDP
- Port Numbers
- Advantages
- Real-world applications

---

# 📑 Table of Contents

- What is the Transport Layer?
- Functions
- TCP
- UDP
- Port Numbers
- Advantages
- Real-World Applications
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is the Transport Layer?

The **Transport Layer** provides communication between applications on different devices.

Its primary responsibility is to ensure that data is delivered to the **correct application** on the destination device.

Depending on the application's requirements, it can provide either:

- Reliable communication using **TCP**
- Fast communication using **UDP**

---

# ⚙️ Functions of the Transport Layer

The Transport Layer performs several important functions:

- End-to-end communication
- Data segmentation
- Data reassembly
- Flow control
- Error detection and recovery
- Reliable data delivery
- Port addressing
- Multiplexing and demultiplexing

---

# 📡 TCP (Transmission Control Protocol)

TCP is a **connection-oriented** protocol that provides reliable communication.

### Features

- Reliable communication
- Error detection
- Flow control
- Ordered delivery
- Retransmission of lost data
- Connection establishment before communication

### Common Applications

- Web Browsing (HTTP/HTTPS)
- Email
- File Transfer
- Online Banking
- Database Communication

---

# 🚀 UDP (User Datagram Protocol)

UDP is a **connectionless** protocol that prioritizes speed over reliability.

### Features

- Faster communication
- No connection establishment
- Lower overhead
- No retransmission
- No guaranteed delivery

### Common Applications

- Live Video Streaming
- Online Gaming
- Voice over IP (VoIP)
- DNS Queries
- Video Conferencing

---

# 🚪 Port Numbers

The Transport Layer uses **port numbers** to identify the destination application.

Common port numbers include:

| Application | Port |
|-------------|-----:|
| HTTP | 80 |
| HTTPS | 443 |
| FTP | 21 |
| SSH | 22 |
| SMTP | 25 |
| DNS | 53 |
| DHCP | 67 / 68 |

Port numbers allow multiple applications to communicate simultaneously over the same network connection.

---

# ✅ Advantages

- Provides reliable communication using TCP.
- Supports fast communication using UDP.
- Ensures data reaches the correct application.
- Supports multiple simultaneous network applications.
- Performs error detection and recovery.

---

# 🌍 Real-World Applications

The Transport Layer is used in:

- Web Browsing
- Email Services
- Cloud Computing
- Online Banking
- Video Streaming
- Online Gaming
- Voice Calls (VoIP)
- File Transfer

---

# 📷 Diagram

![Transport-Layer](https://github.com/varun-kumar-sec/networking-notes/blob/main/TCP-IP%20Model/Four%20Layer%20of%20TCP-IP%20Model/image/Transport-layer.png?raw=true)

---

# 🎤 Interview Questions

### Beginner

- What is the Transport Layer?
- Which protocols operate at the Transport Layer?
- What is the purpose of a port number?
- Which protocol is connection-oriented?

### Intermediate

- Explain the functions of the Transport Layer.
- Differentiate between TCP and UDP.
- Why is TCP considered reliable?
- Give examples of applications that use UDP.

---

# 📌 Key Takeaways

- The Transport Layer is **Layer 3** of the TCP/IP Model.
- It provides end-to-end communication between applications.
- TCP provides reliable communication.
- UDP provides faster communication with lower overhead.
- Port numbers identify destination applications.
- The Transport Layer performs segmentation, flow control, and error recovery.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- RFC 793 – Transmission Control Protocol (TCP)
- RFC 768 – User Datagram Protocol (UDP)
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
