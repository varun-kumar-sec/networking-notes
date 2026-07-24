# Internet Message Access Protocol (IMAP)
# 📖 Overview

The **Internet Message Access Protocol (IMAP)** is an application-layer protocol used by email clients to **retrieve and manage emails stored on a mail server**.

Unlike POP3, which typically downloads emails to a single device, IMAP keeps emails on the server and synchronizes them across multiple devices.

This allows users to access the same mailbox from smartphones, laptops, tablets, and desktop computers while keeping all email folders and read/unread status synchronized.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What is IMAP?
- Why IMAP is used
- How IMAP works
- Default ports
- Advantages and limitations
- Real-world applications

---

# 📑 Table of Contents

- What is IMAP?
- Why is IMAP Needed?
- How IMAP Works
- Default Ports
- Advantages
- Limitations
- Real-World Applications
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is IMAP?

**IMAP (Internet Message Access Protocol)** is a protocol that allows users to access and manage emails directly on a mail server.

Instead of permanently downloading messages, IMAP synchronizes email data between the server and all connected devices.

This means actions such as:

- Reading emails
- Deleting emails
- Moving emails
- Creating folders

are reflected across every device connected to the same email account.

---

# ❓ Why is IMAP Needed?

IMAP is useful because it:

- Synchronizes emails across multiple devices.
- Keeps emails stored on the server.
- Allows access from anywhere with an Internet connection.
- Preserves folder organization.
- Reduces the risk of losing emails stored only on one device.

---

# ⚙️ How IMAP Works

The communication process generally follows these steps:

1. The email client connects to the mail server.
2. The user logs into the email account.
3. The client retrieves the mailbox information.
4. Emails remain stored on the server.
5. Any changes made on one device are synchronized with the server and reflected on other devices.

---

# 📡 Default Ports

| Protocol | Port | Purpose |
|----------|-----:|----------|
| TCP | 143 | Standard IMAP |
| TCP | 993 | Secure IMAP (IMAPS) |

---

# 🔄 IMAP Workflow

```text
Email Client
      │
      │ IMAP Request
      ▼
 Mail Server
      ▲
      │ Email Synchronization
      │
Multiple Devices Stay Updated
```

---

# ✅ Advantages

- Synchronizes emails across multiple devices.
- Emails remain safely stored on the server.
- Supports folder management.
- Allows access from anywhere.
- Ideal for modern cloud-based email services.

---

# ❌ Limitations

- Requires continuous access to the mail server.
- Uses more server storage.
- Synchronization may consume additional bandwidth.
- Performance can depend on Internet connectivity.

---

# 🌍 Real-World Applications

IMAP is commonly used by:

- Gmail
- Microsoft Outlook
- Apple Mail
- Mozilla Thunderbird
- Yahoo Mail
- Mobile email applications
- Enterprise email systems

---

# 📷 Diagram

Save the diagram as:

```text
images/imap-working.png
```

Recommended diagram:

```text
 Laptop
    │
 Smartphone
    │
 Tablet
    │
 Desktop
    │
    ▼
 IMAP Mail Server
    │
 Emails Stored &
 Synchronized
```

Suggested sources:

- https://commons.wikimedia.org/wiki/Category:Internet_Message_Access_Protocol
- https://en.wikipedia.org/wiki/Internet_Message_Access_Protocol

---

# 🎤 Interview Questions

### Beginner

- What is IMAP?
- Which ports does IMAP use?
- Does IMAP download or synchronize emails?
- Why is IMAP preferred for multiple devices?

### Intermediate

- Explain how IMAP works.
- Differentiate between IMAP and POP3.
- Why does IMAP require more server storage?
- What is the purpose of IMAPS?

---

# 📌 Key Takeaways

- IMAP stands for **Internet Message Access Protocol**.
- It allows users to access and synchronize emails stored on a mail server.
- IMAP uses **TCP Port 143** (standard) and **TCP Port 993** (secure).
- Emails remain on the server instead of being permanently downloaded.
- IMAP is ideal for users who access email from multiple devices.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- RFC 9051 – Internet Message Access Protocol (IMAP4rev2)
- RFC 3501 – Internet Message Access Protocol Version 4rev1
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
