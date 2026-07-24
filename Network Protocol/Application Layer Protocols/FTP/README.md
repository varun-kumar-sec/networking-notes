# File Transfer Protocol (FTP)
# 📖 Overview

The **File Transfer Protocol (FTP)** is a standard network protocol used to transfer files between a client and a server over a TCP/IP network.

FTP allows users to upload, download, rename, delete, and manage files on a remote server.

Although FTP is still widely supported, it is considered **insecure** because it transmits usernames, passwords, and data in plain text. For secure file transfers, protocols such as **SFTP** or **FTPS** are preferred.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What is FTP?
- Why FTP is used
- How FTP works
- Active Mode and Passive Mode
- Default ports
- Advantages and limitations
- Real-world applications

---

# 📑 Table of Contents

- What is FTP?
- Why is FTP Needed?
- How FTP Works
- FTP Communication Modes
- Default Ports
- Advantages
- Limitations
- Real-World Applications
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is FTP?

**FTP (File Transfer Protocol)** is a protocol used for transferring files between a client and a server.

It enables users to:

- Upload files
- Download files
- Delete files
- Rename files
- Create directories
- Manage remote files

FTP uses a **client-server architecture**, where an FTP client communicates with an FTP server.

---

# ❓ Why is FTP Needed?

FTP is useful because it:

- Simplifies file transfers over a network.
- Supports large file transfers.
- Allows remote file management.
- Enables centralized file storage.
- Supports authenticated user access.

---

# ⚙️ How FTP Works

FTP communication consists of two separate connections:

## 1. Control Connection

Used to send commands such as:

- Login
- Upload
- Download
- Delete
- Rename

The control connection remains open throughout the session.

---

## 2. Data Connection

Used to transfer the actual files between the client and the server.

A new data connection is created whenever a file transfer occurs.

---

# 🔄 FTP Communication Modes

FTP supports two communication modes.

## Active Mode

- Client connects to **TCP Port 21**.
- Server initiates the data connection using **TCP Port 20**.
- Suitable for networks without strict firewall restrictions.

---

## Passive Mode

- Client initiates both the control connection and the data connection.
- Works better with modern firewalls and NAT devices.
- More commonly used today.

---

# 📡 Default Ports

| Port | Protocol | Purpose |
|------:|----------|----------|
| TCP 21 | FTP | Control Connection |
| TCP 20 | FTP | Data Connection (Active Mode) |

---

# ✅ Advantages

- Easy file uploading and downloading.
- Supports large file transfers.
- Allows remote file management.
- Widely supported across operating systems.
- Simple to configure.

---

# ❌ Limitations

- Transfers usernames and passwords in plain text.
- Data is not encrypted.
- Vulnerable to packet sniffing.
- Not recommended for sensitive information.
- Has largely been replaced by secure alternatives such as **SFTP** and **FTPS**.

---

# 🌍 Real-World Applications

FTP is commonly used for:

- Website file uploads
- Software distribution
- Backup transfers
- File sharing within organizations
- Server administration

---

# 📷 Diagram

![FTP](https://github.com/varun-kumar-sec/networking-notes/blob/main/Network%20Protocol/Image/ftp.jpg?raw=true)

---

# 🎤 Interview Questions

### Beginner

- What is FTP?
- Which ports does FTP use?
- Why does FTP use two connections?
- What is the purpose of the control connection?

### Intermediate

- Differentiate between Active Mode and Passive Mode.
- Why is FTP considered insecure?
- What operations can be performed using FTP?
- Name two secure alternatives to FTP.

---

# 📌 Key Takeaways

- FTP stands for **File Transfer Protocol**.
- It is used to transfer files between a client and a server.
- FTP uses **TCP Port 21** for the control connection.
- **TCP Port 20** is used for the data connection in Active Mode.
- FTP uses separate control and data connections.
- Because FTP does not encrypt data, secure alternatives like **SFTP** and **FTPS** are preferred for sensitive file transfers.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- RFC 959 – File Transfer Protocol
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
