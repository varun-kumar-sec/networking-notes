# Data Encapsulation
# 📖 Overview

**Data Encapsulation** is the process of adding protocol information to data as it moves **down** the layers of the OSI Model before transmission.

Each layer adds its own header (and sometimes a trailer), which contains information required for communication.

At the receiving device, these headers and trailers are removed in the reverse order through a process called **Decapsulation**.

Encapsulation ensures that data reaches the correct destination accurately and efficiently.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What is Data Encapsulation?
- What is Data Decapsulation?
- How data moves through the OSI Model
- Protocol Data Units (PDUs)
- Headers and Trailers
- Advantages of Encapsulation

---

# 📑 Table of Contents

- What is Data Encapsulation?
- What is Data Decapsulation?
- Encapsulation Process
- Protocol Data Units (PDUs)
- Headers and Trailers
- Advantages
- Real-World Example
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is Data Encapsulation?

**Data Encapsulation** is the process in which each OSI layer adds its own control information to the data before passing it to the next lower layer.

This control information is called a **header**.

The Data Link Layer also adds a **trailer**.

These headers and trailers help the receiving device correctly process and deliver the data.

---

# 🌐 What is Data Decapsulation?

**Data Decapsulation** is the reverse process.

As data moves **up** the OSI layers at the receiving device:

- Each layer removes its own header (and trailer).
- Processes the information.
- Passes the remaining data to the next upper layer.

Finally, the original application data reaches the destination application.

---

# ⚙️ Encapsulation Process

The encapsulation process occurs as follows:

## Step 1 — Application Layer

- Creates the original user data.

**PDU:** Data

↓

## Step 2 — Presentation Layer

- Formats, encrypts, or compresses the data.

**PDU:** Data

↓

## Step 3 — Session Layer

- Establishes and manages the communication session.

**PDU:** Data

↓

## Step 4 — Transport Layer

- Divides data into **Segments**.
- Adds the Transport Layer header.

**PDU:** Segment

↓

## Step 5 — Network Layer

- Adds the IP header.
- Creates **Packets**.

**PDU:** Packet

↓

## Step 6 — Data Link Layer

- Adds the MAC header.
- Adds the Frame Trailer.

**PDU:** Frame

↓

## Step 7 — Physical Layer

- Converts the frame into **Bits**.
- Transmits the bits through the communication medium.

**PDU:** Bits

---

# 📦 Protocol Data Units (PDUs)

Each OSI layer has its own Protocol Data Unit (PDU).

| OSI Layer | PDU |
|-----------|-----|
| Application | Data |
| Presentation | Data |
| Session | Data |
| Transport | Segment |
| Network | Packet |
| Data Link | Frame |
| Physical | Bits |

---

# 🏷️ Headers and Trailers

During encapsulation:

| Layer | Adds |
|--------|------|
| Transport | Header |
| Network | Header |
| Data Link | Header + Trailer |
| Physical | Converts Frame into Bits |

The headers contain information such as:

- Source Address
- Destination Address
- Port Number
- Sequence Number
- Error Checking Information

---

# ✅ Advantages of Encapsulation

- Enables communication between different devices.
- Organizes data into manageable units.
- Supports reliable communication.
- Provides addressing information.
- Improves error detection.
- Makes communication modular.

---

# 🌍 Real-World Example

Suppose a user opens a website.

1. The browser creates the request.
2. The Application Layer prepares the data.
3. The Transport Layer creates segments.
4. The Network Layer adds IP addresses.
5. The Data Link Layer adds MAC addresses.
6. The Physical Layer transmits the bits.
7. The receiving device performs **Decapsulation** and delivers the request to the web server.

---

# 📷 Diagram

![Data-Encapsulation](https://github.com/varun-kumar-sec/networking-notes/blob/main/OSI%20Model/Data%20Encapsulation/image/data-encapsulation.jpg?raw=true)

---

# 🎤 Interview Questions

### Beginner

- What is Data Encapsulation?
- What is Data Decapsulation?
- What is a Protocol Data Unit (PDU)?
- Which layer adds a trailer?

### Intermediate

- Explain the encapsulation process.
- Explain the decapsulation process.
- Differentiate between a Segment, Packet, Frame, and Bits.
- Why are headers added at each layer?

---

# 📌 Key Takeaways

- Encapsulation is the process of adding protocol information while data moves down the OSI layers.
- Decapsulation removes this information as data moves up the layers.
- Each layer has its own Protocol Data Unit (PDU).
- The Data Link Layer is the only OSI layer that adds both a **header** and a **trailer**.
- Encapsulation enables reliable and organized communication between devices.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- ISO/IEC 7498-1 (OSI Reference Model)
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
