# Post Office Protocol Version 3 (POP3)
# 📖 Overview

The **Post Office Protocol Version 3 (POP3)** is an application-layer protocol used by email clients to retrieve emails from a mail server.

Unlike protocols that keep emails synchronized on the server, POP3 is designed to **download emails from the mail server to the user's local device**. After downloading, emails are often removed from the server, depending on the email client's configuration.

POP3 is ideal for users who primarily access their email from a single device.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What is POP3?
- Why POP3 is used
- How POP3 works
- Default ports
- Advantages and limitations
- Real-world applications

---

# 📑 Table of Contents

- What is POP3?
- Why is POP3 Needed?
- How POP3 Works
- Default Ports
- Advantages
- Limitations
- Real-World Applications
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is POP3?

**POP3 (Post Office Protocol Version 3)** is a protocol that allows an email client to download emails from a mail server to a local device.

Once downloaded, the emails are stored on the user's computer or mobile device. Depending on the client's settings, the emails may also be deleted from the server.

This approach allows users to read emails even when they are offline.

---

# ❓ Why is POP3 Needed?

POP3 is useful because it:

- Downloads emails for offline access.
- Reduces storage requirements on the mail server.
- Works well for users with a single email device.
- Provides simple email retrieval.

---

# ⚙️ How POP3 Works

The communication process generally follows these steps:

1. The email client connects to the mail server.
2. The user logs into the email account.
3. The client downloads available emails.
4. Emails are stored locally on the device.
5. Depending on the configuration, emails may be removed from the server.

---

# 📡 Default Ports

| Protocol | Port | Purpose |
|----------|-----:|----------|
| TCP | 110 | Standard POP3 |
| TCP | 995 | Secure POP3 (POP3S) |

---

# 🔄 POP3 Workflow

```text
Email Client
      │
      │ POP3 Request
      ▼
 Mail Server
      │
 Downloads Emails
      ▼
 Local Device
```

---

# ✅ Advantages

- Supports offline email access.
- Simple and lightweight protocol.
- Reduces storage usage on the mail server.
- Suitable for single-device email access.
- Easy to configure.

---

# ❌ Limitations

- Emails are primarily stored on the local device.
- Limited synchronization across multiple devices.
- Folder organization on the server is generally not synchronized.
- If local emails are lost and no backup exists, recovery may be difficult.

---

# 🌍 Real-World Applications

POP3 is commonly used in:

- Desktop email clients
- Home computers
- Small office environments
- Networks with limited Internet connectivity
- Users who primarily check email from one device

---

# 📷 Diagram

Save the diagram as:

```text
images/pop3-working.png
```

Recommended diagram:

```text
Email Client
      │
      │ POP3 Request
      ▼
 Mail Server
      │
 Downloads Emails
      ▼
 Local Storage
```

Suggested sources:

- https://commons.wikimedia.org/wiki/Category:Post_Office_Protocol
- https://en.wikipedia.org/wiki/Post_Office_Protocol

---

# 🎤 Interview Questions

### Beginner

- What is POP3?
- Which ports does POP3 use?
- Does POP3 download or synchronize emails?
- Can POP3 be used offline?

### Intermediate

- Explain how POP3 works.
- Why is POP3 suitable for single-device usage?
- What is POP3S?
- What happens to emails after they are downloaded?

---

# 📌 Key Takeaways

- POP3 stands for **Post Office Protocol Version 3**.
- It downloads emails from a mail server to a local device.
- POP3 uses **TCP Port 110** (standard) and **TCP Port 995** (secure).
- It supports offline email access.
- POP3 is best suited for users who primarily access email from one device.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- RFC 1939 – Post Office Protocol Version 3
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
