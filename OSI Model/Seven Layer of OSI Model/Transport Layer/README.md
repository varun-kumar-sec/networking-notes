# Transport Layer
# 📖 Overview

The **Transport Layer** is the **4th layer** of the OSI Model. It is responsible for **end-to-end communication** between applications running on different devices.

This layer ensures that data is delivered **accurately**, **completely**, and **in the correct order**. It also performs **segmentation**, **flow control**, **error control**, and **port addressing**.

The two most common Transport Layer protocols are **TCP (Transmission Control Protocol)** and **UDP (User Datagram Protocol)**.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What is the Transport Layer?
- Functions of the Transport Layer
- TCP and UDP
- Port Numbers
- Advantages of the Transport Layer

---

# 📑 Table of Contents

- What is the Transport Layer?
- Functions
- TCP and UDP
- Port Numbers
- Advantages
- Real-World Applications
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is the Transport Layer?

The **Transport Layer** provides **end-to-end communication** between applications on different devices.

Unlike the Network Layer, which delivers packets between networks, the Transport Layer ensures that the **entire message reaches the correct application** on the destination device.

At this layer, data is divided into **segments** before transmission and reassembled at the receiving end.

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

# ✂️ Segmentation and Reassembly

Large amounts of data are divided into **smaller segments** before transmission.

After reaching the destination:

- The segments are reassembled.
- The original message is reconstructed.

This makes data transmission more efficient and reliable.

---

# 🔄 Flow Control

Flow control ensures that:

- A fast sender does not overwhelm a slow receiver.
- Data is transmitted at an appropriate rate.

This prevents packet loss due to receiver overload.

---

# ✔️ Error Control

The Transport Layer detects transmission errors.

If data is lost or corrupted:

- The receiver requests retransmission.
- The sender sends the missing segment again.

This ensures reliable communication.

---

# 🚪 Port Numbers

The Transport Layer uses **Port Numbers** to identify the destination application on a device.

Examples:

| Application | Default Port |
|-------------|-------------:|
| HTTP | 80 |
| HTTPS | 443 |
| FTP | 21 |
| SSH | 22 |
| SMTP | 25 |
| DNS | 53 |

Port numbers allow multiple applications to communicate simultaneously on the same computer.

---

# 📡 TCP and UDP

## TCP (Transmission Control Protocol)

TCP is a **connection-oriented** protocol.

### Features

- Reliable communication
- Error checking
- Flow control
- Ordered data delivery
- Retransmission of lost data

### Used In

- Web Browsing (HTTP/HTTPS)
- Email
- File Transfer
- Online Banking

---

## UDP (User Datagram Protocol)

UDP is a **connectionless** protocol.

### Features

- Faster communication
- No retransmission
- Lower overhead
- No guarantee of delivery

### Used In

- Live Video Streaming
- Voice over IP (VoIP)
- Online Gaming
- DNS Queries

---

# ✅ Advantages

- Provides reliable end-to-end communication.
- Supports multiple applications using port numbers.
- Performs flow control and error recovery.
- Ensures ordered delivery of data.
- Supports both reliable (TCP) and fast (UDP) communication.

---

# 🌍 Real-World Applications

The Transport Layer is used in:

- Web Browsing
- Email Communication
- File Transfer
- Video Streaming
- Online Gaming
- Voice Calls (VoIP)
- Cloud Applications

---

# 📷 Diagram

![Transport-Layer](https://github.com/varun-kumar-sec/networking-notes/blob/main/OSI%20Model/Seven%20Layer%20of%20OSI%20Model/image/Transport-Layer.png?raw=true)

---

# 🎤 Interview Questions

### Beginner

- Which layer is the Transport Layer?
- What is the primary function of the Transport Layer?
- What is the data unit of the Transport Layer?
- Name the two Transport Layer protocols.

### Intermediate

- Explain the functions of the Transport Layer.
- Differentiate between TCP and UDP.
- What is a port number?
- Why is TCP considered reliable?

---

# 📌 Key Takeaways

- The Transport Layer is **Layer 4** of the OSI Model.
- It provides **end-to-end communication**.
- Data is divided into **segments**.
- It performs segmentation, flow control, error control, and reassembly.
- It uses **port numbers** to identify applications.
- TCP provides reliable communication, while UDP provides faster communication with lower overhead.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- RFC 793 – Transmission Control Protocol (TCP)
- RFC 768 – User Datagram Protocol (UDP)
- ISO/IEC 7498-1 (OSI Reference Model)
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
