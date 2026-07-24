# What is a Port?
# 📖 Overview

A **Port** is a **logical communication endpoint** used by the Transport Layer to identify a specific application or service running on a device.

While an **IP address** identifies a device on a network, a **port number** identifies the application or service on that device.

For example, a web server and an email server can run on the same computer because they listen on different port numbers.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What is a port?
- Why ports are needed
- How port numbers work
- Types of port numbers
- Common well-known ports
- Real-world examples

---

# 📑 Table of Contents

- What is a Port?
- Why are Ports Needed?
- How Ports Work
- Types of Port Numbers
- Common Port Numbers
- Advantages
- Real-World Applications
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is a Port?

A **Port** is a numerical identifier that allows a computer to send data to the correct application.

Think of it like an apartment building:

- **IP Address** → Building Address
- **Port Number** → Apartment Number

The building (device) may be the same, but each apartment (application) is different.

For example:

- A web browser communicates with a web server using **Port 80** or **443**.
- An email application communicates using **Port 25**, **110**, or **143**.

---

# ❓ Why are Ports Needed?

Ports are necessary because multiple applications can use the network at the same time.

Without ports, a computer would not know which application should receive incoming data.

Ports help:

- Identify applications.
- Support multiple simultaneous network connections.
- Organize network communication.
- Enable efficient data delivery.

---

# ⚙️ How Ports Work

When data is sent across a network:

1. The sender specifies the destination IP address.
2. The sender also specifies a destination port number.
3. The receiving device checks the port number.
4. The operating system forwards the data to the correct application.

This process is handled by the **Transport Layer** using **TCP** or **UDP**.

---

# 🔢 Types of Port Numbers

Port numbers range from **0 to 65535** and are divided into three categories.

## 1. Well-Known Ports (0–1023)

Reserved for common Internet services.

Examples:

- HTTP (80)
- HTTPS (443)
- FTP (21)
- SSH (22)
- DNS (53)

---

## 2. Registered Ports (1024–49151)

Assigned to user applications and software vendors.

Examples include database services, game servers, and application-specific services.

---

## 3. Dynamic / Private Ports (49152–65535)

Used temporarily by client applications when initiating network communication.

These are also known as **Ephemeral Ports**.

---

# 📋 Common Well-Known Port Numbers

| Port | Protocol | Purpose |
|------:|----------|----------|
| 20 | FTP | Data Transfer |
| 21 | FTP | Control Connection |
| 22 | SSH | Secure Remote Login |
| 23 | Telnet | Remote Login |
| 25 | SMTP | Send Email |
| 53 | DNS | Domain Name Resolution |
| 67 | DHCP | Server |
| 68 | DHCP | Client |
| 69 | TFTP | File Transfer |
| 80 | HTTP | Web Browsing |
| 110 | POP3 | Receive Email |
| 143 | IMAP | Email Synchronization |
| 161 | SNMP | Network Management |
| 443 | HTTPS | Secure Web Browsing |

---

# ✅ Advantages

- Identifies network applications.
- Allows multiple services on one device.
- Organizes network communication.
- Supports simultaneous connections.
- Simplifies data delivery.

---

# 🌍 Real-World Applications

Ports are used whenever you:

- Browse websites
- Send emails
- Download files
- Access remote servers
- Use cloud applications
- Play online games
- Stream videos

---

# 📷 Diagram

![network-ports](https://github.com/varun-kumar-sec/networking-notes/blob/main/Network%20Protocol/Image/networks_ports.Png?raw=true)

---

# 🎤 Interview Questions

### Beginner

- What is a port?
- Why are port numbers used?
- What is the range of port numbers?
- Which layer uses port numbers?

### Intermediate

- Differentiate between an IP address and a port number.
- Explain the three categories of port numbers.
- What are ephemeral ports?
- Why can multiple applications use the same IP address?

---

# 📌 Key Takeaways

- A port is a logical communication endpoint used to identify applications.
- IP addresses identify devices, while port numbers identify services.
- Port numbers range from **0 to 65535**.
- They are divided into **Well-Known**, **Registered**, and **Dynamic** ports.
- TCP and UDP use port numbers to deliver data to the correct application.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- IANA Service Name and Port Number Registry
- RFC 6335 – Internet Assigned Numbers Authority (IANA)
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
