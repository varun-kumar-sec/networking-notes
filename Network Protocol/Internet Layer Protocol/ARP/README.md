# Address Resolution Protocol (ARP)
# 📖 Overview

The **Address Resolution Protocol (ARP)** is a protocol used to determine the **MAC address** of a device when its **IP address** is already known.

Computers communicate over local networks using **MAC addresses**, while users and applications typically work with **IP addresses**. ARP acts as the bridge between these two addressing schemes by translating an IPv4 address into its corresponding MAC address.

Without ARP, devices on the same Local Area Network (LAN) would not know where to send Ethernet frames.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What is ARP?
- Why ARP is needed
- How ARP works
- ARP Request and ARP Reply
- ARP Cache
- Advantages and limitations
- Real-world applications

---

# 📑 Table of Contents

- What is ARP?
- Why is ARP Needed?
- How ARP Works
- ARP Cache
- Advantages
- Limitations
- Real-World Applications
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is ARP?

**ARP (Address Resolution Protocol)** is a protocol that maps an **IPv4 address** to a **MAC address** within a local network.

For example:

```text
IP Address:
192.168.1.10

↓

MAC Address:
00:1A:2B:3C:4D:5E
```

This mapping allows Ethernet frames to be delivered to the correct device on the LAN.

---

# ❓ Why is ARP Needed?

ARP is important because:

- Devices communicate locally using MAC addresses.
- Applications identify devices using IP addresses.
- ARP connects these two addressing methods.
- It enables successful communication within a LAN.

---

# ⚙️ How ARP Works

The ARP process generally follows these steps:

### Step 1

A device wants to communicate with another device whose IP address is known.

↓

### Step 2

The sender checks its **ARP Cache** to see if the corresponding MAC address is already stored.

↓

### Step 3

If no entry exists, the sender broadcasts an **ARP Request** asking:

> "Who has this IP address?"

↓

### Step 4

The device with that IP address responds with an **ARP Reply** containing its MAC address.

↓

### Step 5

The sender stores the information in its ARP Cache and begins communication.

---

# 🗂️ ARP Cache

An **ARP Cache** is a temporary table maintained by the operating system.

It stores recently learned IP-to-MAC address mappings.

Using the ARP Cache avoids sending an ARP Request every time communication occurs, improving network efficiency.

---

# 📡 ARP Request and Reply

### ARP Request

- Broadcast message
- Sent to every device on the local network
- Asks for the MAC address of a specific IP address

### ARP Reply

- Unicast message
- Sent directly to the requesting device
- Contains the requested MAC address

---

# ✅ Advantages

- Automatically resolves IP addresses to MAC addresses.
- Eliminates manual address mapping.
- Enables local network communication.
- Improves efficiency through ARP caching.
- Simple and lightweight protocol.

---

# ❌ Limitations

- Works only within a local network.
- Supports only IPv4.
- Broadcast requests can increase network traffic.
- Vulnerable to ARP Spoofing (ARP Poisoning) attacks.

---

# 🌍 Real-World Applications

ARP is commonly used in:

- Home networks
- Office LANs
- Ethernet communication
- Router communication
- Switch communication
- Local device discovery

---

# 📷 Diagram

Save the diagram as:

```text
images/arp-working.png
```

Recommended diagram:

```text
Computer A
(IP: 192.168.1.2)
      │
      │ ARP Request (Broadcast)
      ▼
"Who has 192.168.1.10?"

---------------- LAN ----------------

Computer B
(IP: 192.168.1.10)
(MAC: 00:1A:2B:3C:4D:5E)

      │
      │ ARP Reply (Unicast)
      ▼

MAC Address Returned
```

Suggested sources:

- https://commons.wikimedia.org/wiki/Category:Address_Resolution_Protocol
- https://en.wikipedia.org/wiki/Address_Resolution_Protocol

---

# 🎤 Interview Questions

### Beginner

- What is ARP?
- Why is ARP needed?
- What information does ARP resolve?
- What is an ARP Cache?

### Intermediate

- Explain the ARP Request and Reply process.
- Why is the ARP Request broadcast?
- Why is the ARP Reply unicast?
- What is ARP Spoofing?
- Does ARP work with IPv6?

---

# 📌 Key Takeaways

- ARP stands for **Address Resolution Protocol**.
- It maps an **IPv4 address** to a **MAC address**.
- ARP is used only within a **Local Area Network (LAN)**.
- Communication begins with an **ARP Request** and ends with an **ARP Reply**.
- Devices store mappings in an **ARP Cache** for faster future communication.
- ARP is essential for Ethernet communication in IPv4 networks.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- RFC 826 – Address Resolution Protocol
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
