# What is FTP?
# 📖 Overview

**FTP (File Transfer Protocol)** is a network protocol used to transfer files between a client and a server over a network.

FTP allows users to **upload, download, rename, delete, and manage files** on a remote server, depending on the permissions assigned to their account.

FTP follows a **client-server architecture**, where the FTP client connects to an FTP server to perform file transfer operations.

FTP is commonly associated with website management, file distribution, and transferring files between systems.

> **Important:** Standard FTP does **not encrypt** usernames, passwords, or transferred data. For secure file transfers, technologies such as **SFTP** or **FTPS** should be considered.

---

# 🎯 Learning Objectives

After completing this topic, you will be able to:

* Understand what FTP is.
* Explain how FTP works.
* Understand FTP client-server architecture.
* Identify common FTP operations.
* Understand FTP ports.
* Differentiate FTP from SFTP and FTPS.
* Identify basic FTP security concerns.

---

# 📑 Table of Contents

* What is FTP?
* Why FTP is Used
* How FTP Works
* FTP Client and Server
* FTP Ports
* Common FTP Operations
* FTP Connection Modes
* FTP vs SFTP vs FTPS
* FTP Security
* Real-World Applications
* Diagram
* Interview Questions
* Key Takeaways
* References

---

# 🌐 What is FTP?

**File Transfer Protocol (FTP)** is a standard protocol designed to transfer files between computers over a TCP/IP network.

FTP uses a client-server model:

```text
FTP Client  ───────────────►  FTP Server
            File Transfer
```

The client initiates a connection to the server and requests operations such as uploading or downloading files.

---

# 💡 Why FTP is Used

FTP can be used to:

* Upload files to a remote server.
* Download files from a server.
* Manage files and directories remotely.
* Transfer large numbers of files.
* Distribute files to multiple users.
* Manage website files on a hosting server.

For example, a web developer can use an FTP client to upload website files to a web server.

---

# ⚙️ How FTP Works

A basic FTP connection works as follows:

1. The FTP client starts a connection.
2. The client connects to the FTP server.
3. The server requests authentication if required.
4. The user provides credentials.
5. The server verifies the credentials.
6. The client can perform permitted file operations.
7. Files are transferred between the client and server.
8. The connection is closed when the session is finished.

---

# 🖥️ FTP Client and FTP Server

## FTP Client

An **FTP client** is software used to connect to an FTP server.

Examples include:

* FileZilla
* WinSCP
* Command-line FTP clients

The client provides an interface for uploading, downloading, and managing files.

---

## FTP Server

An **FTP server** is a computer or service that stores files and accepts FTP connections from clients.

The server controls:

* User authentication.
* File access.
* Directory access.
* Upload permissions.
* Download permissions.
* File management operations.

---

# 🔌 FTP Ports

FTP commonly uses **TCP port 21** for the control connection.

A separate connection is used for transferring data.

| Connection | Port / Mechanism    | Purpose                     |
| ---------- | ------------------- | --------------------------- |
| Control    | TCP 21              | Commands and authentication |
| Data       | Depends on FTP mode | File and directory data     |

FTP has two main connection modes:

* Active FTP
* Passive FTP

The data connection behaves differently depending on the selected mode.

---

# 📤 Common FTP Operations

FTP supports several common operations.

### Upload

Transfers a file from the client to the server.

```text
Client ─────────► Server
       Upload
```

### Download

Transfers a file from the server to the client.

```text
Client ◄───────── Server
       Download
```

### Directory Listing

Displays files and folders available on the server.

### Rename

Changes the name of a file or directory when permitted.

### Delete

Removes a file or directory when the account has the required permissions.

---

# 🔄 FTP Connection Modes

## Active FTP

In **active mode**, the FTP server establishes the data connection back to the client.

Simplified flow:

```text
Client ─────► Server
   Control

Server ─────► Client
     Data
```

Active FTP can encounter problems with client-side firewalls or NAT because the server must establish a connection back toward the client.

---

## Passive FTP

In **passive mode**, the client establishes both the control and data connections.

```text
Client ─────► Server
   Control

Client ─────► Server
     Data
```

Passive FTP is commonly preferred when clients are behind NAT routers or firewalls because the client initiates the connections.

---

# 🔐 FTP vs SFTP vs FTPS

These protocols are related but are **not the same technology**.

| Feature               | FTP                    | FTPS       | SFTP                       |
| --------------------- | ---------------------- | ---------- | -------------------------- |
| Full Name             | File Transfer Protocol | FTP Secure | SSH File Transfer Protocol |
| Encryption            | ❌ No                   | ✅ TLS/SSL  | ✅ SSH                      |
| Common Port           | TCP 21                 | TCP 21     | TCP 22                     |
| Secure Authentication | ❌ Not by itself        | ✅          | ✅                          |
| Based On              | FTP                    | FTP + TLS  | SSH                        |

### FTP

Standard FTP does not encrypt credentials or transferred data.

### FTPS

FTPS adds **TLS encryption** to FTP.

### SFTP

SFTP is a different protocol that operates over **SSH**. It is not simply "secure FTP."

---

# 🛡️ FTP Security

Standard FTP has significant security limitations.

## Credentials Are Not Encrypted

Usernames and passwords can be transmitted without encryption.

## Data Is Not Encrypted

Files transferred using standard FTP can potentially be intercepted.

## Firewall Considerations

FTP may require additional firewall and NAT configuration because it uses separate control and data connections.

## Recommended Alternatives

For sensitive information, use:

* SFTP
* FTPS
* Other secure file transfer solutions

Avoid standard FTP for transmitting sensitive credentials or confidential information across untrusted networks.

---

# 💼 Real-World Applications

FTP and related technologies have historically been used for:

* Website file management.
* Software distribution.
* Server administration.
* Large file transfers.
* Backup file transfers.
* File exchange between systems.

Modern environments often prefer **SFTP**, **FTPS**, HTTPS-based transfers, or cloud storage when security is important.

---

# 📷 Diagram

![what-is-FTP](https://github.com/varun-kumar-sec/networking-notes/blob/main/File%20Sharing%20and%20Troubleshooting/Image/FTP.png?raw=true)

---

# 🎤 Interview Questions

### Beginner

* What is FTP?
* What does FTP stand for?
* What is the purpose of FTP?
* What is an FTP client?
* What is an FTP server?
* Which port does FTP commonly use for its control connection?

### Intermediate

* Explain how FTP works.
* What is the difference between active and passive FTP?
* Why is standard FTP considered insecure?
* What is the difference between FTP, FTPS, and SFTP?
* Why is passive FTP commonly used behind NAT?
* Which protocol would you choose for secure file transfers?

---

# 📌 Key Takeaways

* **FTP stands for File Transfer Protocol.**
* FTP uses a client-server architecture to transfer files.
* TCP port **21** is commonly used for the FTP control connection.
* FTP supports operations such as uploading, downloading, renaming, and deleting files.
* FTP has **active** and **passive** connection modes.
* Standard FTP does not encrypt credentials or transferred data.
* **FTPS** secures FTP using TLS.
* **SFTP** is a separate file transfer protocol that operates over SSH.
* Secure alternatives should be used when transferring sensitive information.

---

# 📚 References

* RFC 959 – File Transfer Protocol
* RFC 4217 – Securing FTP with TLS
* RFC 4253 – SSH Transport Layer Protocol
* Microsoft Learn – Windows Networking Documentation
* Cisco Networking Academy (NetAcad)
* CompTIA Network+
* Andrew S. Tanenbaum – *Computer Networks*
* Behrouz A. Forouzan – *Data Communications and Networking*
*
