# Data Encapsulation in the TCP/IP Model
# 📖 Overview

**Data Encapsulation** in the TCP/IP Model is the process of adding protocol-specific information to data as it moves through the four layers before transmission over a network.

Each layer adds its own **header**, which contains information required for successful communication. At the receiving device, these headers are removed in the reverse order through a process called **Decapsulation**.

This process enables reliable communication between devices across local and global networks, including the Internet.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What is Data Encapsulation?
- What is Data Decapsulation?
- How data moves through the TCP/IP Model
- Protocol Data Units (PDUs)
- Headers added at each layer
- Advantages of Encapsulation

---

# 📑 Table of Contents

- What is Data Encapsulation?
- What is Data Decapsulation?
- Encapsulation Process
- Protocol Data Units (PDUs)
- Headers Added by Each Layer
- Advantages
- Real-World Example
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is Data Encapsulation?

**Data Encapsulation** is the process of preparing data for transmission by adding protocol information at each layer of the TCP/IP Model.

Each layer adds a **header** containing information required for communication. As the data moves down the TCP/IP stack, it becomes ready for transmission across the network.

---

# 🌐 What is Data Decapsulation?

**Data Decapsulation** is the reverse process.

When the data reaches the destination device:

- Each TCP/IP layer removes its own header.
- Processes the information.
- Passes the remaining data to the next upper layer.

Finally, the original application data reaches the destination application.

---

# ⚙️ Encapsulation Process

The TCP/IP encapsulation process occurs as follows:

## Step 1 — Application Layer

- Creates the user data.
- Adds application-specific information.

**PDU:** Data

↓

## Step 2 — Transport Layer

- Divides the data into **Segments**.
- Adds the TCP or UDP header.

**PDU:** Segment

↓

## Step 3 — Internet Layer

- Adds the IP header.
- Creates **Packets**.

**PDU:** Packet

↓

## Step 4 — Network Access Layer

- Adds the Frame Header and Trailer.
- Converts the frame into **Bits** for transmission over the communication medium.

**PDU:** Frame → Bits

---

# 📦 Protocol Data Units (PDUs)

Each TCP/IP layer uses a specific Protocol Data Unit (PDU).

| TCP/IP Layer | PDU |
|---------------|-----|
| Application | Data |
| Transport | Segment |
| Internet | Packet |
| Network Access | Frame → Bits |

---

# 🏷️ Headers Added by Each Layer

During encapsulation:

| Layer | Header Added |
|--------|--------------|
| Application | Application-specific information |
| Transport | TCP or UDP Header |
| Internet | IP Header |
| Network Access | Frame Header + Trailer |

These headers contain information such as:

- Source Address
- Destination Address
- Port Number
- Sequence Number
- Protocol Information
- Error Detection Information

---

# ✅ Advantages of Encapsulation

- Organizes data for transmission.
- Enables communication across different networks.
- Supports reliable delivery using TCP.
- Allows efficient routing using IP.
- Provides addressing information.
- Supports error detection and recovery.

---

# 🌍 Real-World Example

Suppose a user visits a website.

1. The browser creates an HTTP request.
2. The Application Layer prepares the data.
3. The Transport Layer creates TCP segments.
4. The Internet Layer adds IP addresses.
5. The Network Access Layer adds MAC addresses and transmits the data as bits.
6. The destination device performs **Decapsulation** to recover the original request.

---

# 📷 Diagram

Save the diagram as:

```text
images/tcp-ip-encapsulation.png
```

Recommended diagram:

```text
Sender

Application Layer
        │
      Data
        ↓
Transport Layer
        │
    Segment
        ↓
Internet Layer
        │
     Packet
        ↓
Network Access Layer
        │
 Frame → Bits
=========================
Network Transmission
=========================

Receiver

Bits
 ↑
Frame
 ↑
Packet
 ↑
Segment
 ↑
Data
```

Suggested sources:

- https://commons.wikimedia.org/wiki/Category:TCP/IP
- https://en.wikipedia.org/wiki/Internet_protocol_suite

---

# 🎤 Interview Questions

### Beginner

- What is Data Encapsulation?
- What is Data Decapsulation?
- What is the PDU of the Internet Layer?
- Which layer adds the IP header?

### Intermediate

- Explain the encapsulation process in the TCP/IP Model.
- What headers are added at each layer?
- Why is encapsulation important?
- Differentiate between encapsulation and decapsulation.

---

# 📌 Key Takeaways

- Encapsulation prepares data for network transmission.
- Each TCP/IP layer adds its own protocol header.
- The Transport Layer creates segments.
- The Internet Layer creates packets.
- The Network Access Layer creates frames and transmits bits.
- Decapsulation removes the headers at the receiving device to recover the original data.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- RFC 791 – Internet Protocol (IP)
- RFC 793 – Transmission Control Protocol (TCP)
- RFC 768 – User Datagram Protocol (UDP)
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
