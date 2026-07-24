# Telnet
# 📖 Overview

**Telnet** is an application-layer protocol that allows users to remotely access and manage another computer or network device over a TCP/IP network.

It provides a command-line interface (CLI), enabling administrators to configure and troubleshoot remote devices such as routers, switches, and servers.

Since Telnet transmits all data, including usernames and passwords, in plain text, it is considered **insecure** and has largely been replaced by **SSH (Secure Shell)** for remote administration.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What is Telnet?
- Why Telnet is used
- How Telnet works
- Default port
- Advantages and limitations
- Real-world applications

---

# 📑 Table of Contents

- What is Telnet?
- Why is Telnet Needed?
- How Telnet Works
- Default Port
- Advantages
- Limitations
- Real-World Applications
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is Telnet?

**Telnet** is a protocol that allows a user to establish a remote command-line session with another device over a network.

Using Telnet, administrators can:

- Log in to remote devices.
- Configure network equipment.
- Troubleshoot network issues.
- Execute command-line operations.

Telnet follows a **client-server architecture**, where a Telnet client connects to a Telnet server running on the remote device.

---

# ❓ Why is Telnet Needed?

Telnet is useful because it:

- Enables remote device management.
- Eliminates the need for physical access.
- Simplifies network administration.
- Allows command-line configuration from anywhere on the network.

Although still supported by many devices, Telnet is generally used only in trusted or lab environments.

---

# ⚙️ How Telnet Works

The communication process generally follows these steps:

1. The Telnet client connects to the remote device.
2. The server requests user authentication.
3. The user enters login credentials.
4. After successful authentication, a remote command-line session is established.
5. Commands entered by the user are executed on the remote device, and the results are returned to the client.

---

# 📡 Default Port

| Protocol | Port |
|----------|-----:|
| TCP | 23 |

---

# ✅ Advantages

- Simple remote access protocol.
- Easy to configure.
- Supports remote device management.
- Useful for testing network services.
- Widely supported by legacy systems.

---

# ❌ Limitations

- No encryption.
- Usernames and passwords are transmitted in plain text.
- Vulnerable to packet sniffing and unauthorized access.
- Not recommended for use over public or untrusted networks.
- Largely replaced by SSH for secure remote administration.

---

# 🌍 Real-World Applications

Telnet is commonly used for:

- Networking laboratories
- Legacy network equipment
- Basic connectivity testing
- Learning remote device management
- Troubleshooting simple network services

---

# 📷 Diagram

Save the diagram as:

```text
images/telnet-working.png
```

Recommended diagram:

```text
Telnet Client
      │
      │ TCP Port 23
      ▼
Telnet Server
      │
Remote Command-Line Session
      ▼
Network Device
```

Suggested sources:

- https://commons.wikimedia.org/wiki/Category:Telnet
- https://en.wikipedia.org/wiki/Telnet

---

# 🎤 Interview Questions

### Beginner

- What is Telnet?
- Which port does Telnet use?
- Which transport protocol does Telnet use?
- What is the primary purpose of Telnet?

### Intermediate

- Explain how Telnet works.
- Why is Telnet considered insecure?
- Why has SSH largely replaced Telnet?
- Where is Telnet still commonly used?

---

# 📌 Key Takeaways

- Telnet is an application-layer protocol used for remote command-line access.
- It uses **TCP Port 23**.
- Telnet enables administrators to remotely configure and manage network devices.
- Because Telnet transmits data in plain text, it is considered insecure.
- Modern networks generally use **SSH** instead of Telnet for secure remote administration.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- RFC 854 – Telnet Protocol Specification
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
