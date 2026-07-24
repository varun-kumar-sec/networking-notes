# Simple Mail Transfer Protocol (SMTP)
# 📖 Overview

The **Simple Mail Transfer Protocol (SMTP)** is an application-layer protocol used to **send emails** across a network.

SMTP is responsible for transferring outgoing email messages from an email client to a mail server and between mail servers until they reach the recipient's mail server.

Unlike POP3 and IMAP, SMTP is **not used for reading or retrieving emails**. Its primary role is sending and forwarding email messages.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What is SMTP?
- Why SMTP is used
- How SMTP works
- Default ports
- Advantages and limitations
- Real-world applications

---

# 📑 Table of Contents

- What is SMTP?
- Why is SMTP Needed?
- How SMTP Works
- Default Ports
- Advantages
- Limitations
- Real-World Applications
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is SMTP?

**SMTP (Simple Mail Transfer Protocol)** is the standard protocol used for sending email messages.

SMTP is responsible for:

- Sending emails from an email client to a mail server.
- Forwarding emails between mail servers.
- Delivering outgoing email messages.

After the email reaches the recipient's mail server, protocols such as **POP3** or **IMAP** are used to retrieve it.

---

# ❓ Why is SMTP Needed?

SMTP is important because it:

- Standardizes email transmission.
- Enables communication between different email systems.
- Transfers emails across the Internet.
- Supports reliable email delivery between mail servers.

---

# ⚙️ How SMTP Works

The SMTP communication process generally follows these steps:

1. The sender composes an email.
2. The email client sends the message to the outgoing SMTP server.
3. The SMTP server forwards the email to the recipient's mail server.
4. The recipient's mail server stores the email.
5. The recipient retrieves the email using POP3 or IMAP.

---

# 📡 Default Ports

| Protocol | Port | Purpose |
|----------|-----:|----------|
| TCP | 25 | Standard SMTP (Server-to-Server Communication) |
| TCP | 587 | Mail Submission (Recommended for Clients) |
| TCP | 465 | Secure SMTP (SMTPS) |

---

# 🔄 SMTP Workflow

```text
Sender
   │
   ▼
Email Client
   │
   │ SMTP
   ▼
Outgoing Mail Server
   │
   ▼
Recipient Mail Server
   │
   ▼
Recipient Retrieves Email
(using POP3 or IMAP)
```

---

# ✅ Advantages

- Standard protocol for email transmission.
- Reliable mail delivery.
- Widely supported by email providers.
- Enables communication between different mail servers.
- Simple and efficient.

---

# ❌ Limitations

- Cannot retrieve emails.
- Standard SMTP does not encrypt messages.
- Requires additional protocols such as POP3 or IMAP for email access.
- May require authentication to prevent unauthorized use.

---

# 🌍 Real-World Applications

SMTP is used in:

- Gmail
- Microsoft Outlook
- Yahoo Mail
- Apple Mail
- Thunderbird
- Enterprise email systems
- Corporate mail servers

---

# 📷 Diagram

Save the diagram as:

```text
images/smtp-working.png
```

Recommended diagram:

```text
Sender
   │
Email Client
   │ SMTP
   ▼
Outgoing Mail Server
   │
   ▼
Recipient Mail Server
   │
POP3 / IMAP
   ▼
Recipient
```

Suggested sources:

- https://commons.wikimedia.org/wiki/Category:Simple_Mail_Transfer_Protocol
- https://en.wikipedia.org/wiki/Simple_Mail_Transfer_Protocol

---

# 🎤 Interview Questions

### Beginner

- What is SMTP?
- Which ports does SMTP use?
- Is SMTP used to send or receive emails?
- Which protocols retrieve emails after SMTP delivers them?

### Intermediate

- Explain how SMTP works.
- Differentiate between SMTP Port 25 and Port 587.
- Why is SMTP used together with POP3 or IMAP?
- What is SMTPS?

---

# 📌 Key Takeaways

- SMTP stands for **Simple Mail Transfer Protocol**.
- It is used for **sending and forwarding emails**.
- SMTP uses **TCP Port 25**, **TCP Port 587**, and **TCP Port 465**.
- SMTP transfers emails between clients and mail servers, and between mail servers.
- POP3 and IMAP are used to retrieve emails after SMTP has delivered them.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- RFC 5321 – Simple Mail Transfer Protocol
- RFC 6409 – Message Submission for Mail
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
