# Trivial File Transfer Protocol (TFTP)
# 📖 Overview

The **Trivial File Transfer Protocol (TFTP)** is a lightweight application-layer protocol used to transfer files between devices over a network.

Unlike FTP, TFTP is designed to be **simple and lightweight**, making it suitable for tasks such as transferring configuration files, firmware updates, and boot files.

TFTP does not provide user authentication or encryption, making it suitable only for trusted local networks.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What is TFTP?
- Why TFTP is used
- How TFTP works
- Default port
- Advantages and limitations
- Real-world applications

---

# 📑 Table of Contents

- What is TFTP?
- Why is TFTP Needed?
- How TFTP Works
- Default Port
- Advantages
- Limitations
- Real-World Applications
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is TFTP?

**TFTP (Trivial File Transfer Protocol)** is a simplified file transfer protocol that enables devices to transfer files across a network.

It is commonly used for:

- Transferring configuration files
- Uploading firmware
- Downloading firmware
- Network booting (PXE Boot)
- Backing up router and switch configurations

TFTP focuses on simplicity rather than advanced features.

---

# ❓ Why is TFTP Needed?

TFTP is useful because it:

- Provides simple file transfer.
- Requires minimal resources.
- Supports network device configuration.
- Enables network booting.
- Is easy to implement.

---

# ⚙️ How TFTP Works

The communication process generally follows these steps:

1. A client sends a request to the TFTP server.
2. The server checks whether the requested file exists.
3. The file is transferred in small data blocks.
4. The client acknowledges each received block.
5. The transfer continues until the entire file is delivered.

Because TFTP uses UDP, it performs its own simple acknowledgment mechanism instead of relying on TCP.

---

# 📡 Default Port

| Protocol | Port |
|----------|-----:|
| UDP | 69 |

---

# ✅ Advantages

- Lightweight protocol.
- Easy to configure.
- Requires very little memory.
- Suitable for embedded devices.
- Ideal for firmware and configuration transfers.
- Supports network boot environments.

---

# ❌ Limitations

- No user authentication.
- No encryption.
- Limited functionality.
- Less reliable than TCP-based file transfer protocols.
- Not recommended for transferring sensitive files over public networks.

---

# 🌍 Real-World Applications

TFTP is commonly used for:

- Router configuration backup
- Switch configuration backup
- Firmware upgrades
- BIOS and device updates
- PXE network booting
- Embedded systems
- Network appliance deployment

---

# 📷 Diagram

Save the diagram as:

```text
images/tftp-working.png
```

Recommended diagram:

```text
TFTP Client
      │
      │ Request File
      ▼
 TFTP Server
      │
      │ File Transfer (UDP)
      ▼
TFTP Client
```

Suggested sources:

- https://commons.wikimedia.org/wiki/Category:Trivial_File_Transfer_Protocol
- https://en.wikipedia.org/wiki/Trivial_File_Transfer_Protocol

---

# 🎤 Interview Questions

### Beginner

- What is TFTP?
- Which port does TFTP use?
- Which transport protocol does TFTP use?
- Why is TFTP called a "Trivial" File Transfer Protocol?

### Intermediate

- Explain how TFTP works.
- Why is TFTP commonly used for firmware upgrades?
- Why is TFTP considered insecure?
- Where is TFTP commonly used in networking?

---

# 📌 Key Takeaways

- TFTP stands for **Trivial File Transfer Protocol**.
- It is a lightweight protocol used for simple file transfers.
- TFTP uses **UDP Port 69**.
- It is commonly used for firmware updates, configuration backups, and PXE booting.
- Because TFTP does not provide authentication or encryption, it should only be used in trusted networks.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- RFC 1350 – The TFTP Protocol
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
