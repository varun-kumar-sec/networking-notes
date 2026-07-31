# Confidentiality
# 📖 Overview

**Confidentiality** is the security principle of ensuring that information is accessible only to **authorized users, devices, or systems**. It protects sensitive information from unauthorized access, disclosure, copying, or interception.

Confidentiality is one of the three components of the **CIA Triad**, along with Integrity and Availability.

---

# 🎯 Learning Objectives

After completing this section, you will be able to:

- Understand the meaning of confidentiality.
- Explain why confidentiality is important.
- Identify common threats to confidentiality.
- Identify methods used to protect confidential information.
- Understand the relationship between confidentiality, authentication, and access control.

---

# 📚 Topics Covered

This section includes:

- What is Confidentiality?
- Importance of Confidentiality
- Threats to Confidentiality
- Methods of Protecting Confidentiality
- Confidentiality in Network Communication
- Real-World Applications

---

# 🔐 What is Confidentiality?

Confidentiality ensures that sensitive information is not accessed or disclosed to unauthorized individuals.

### Example

A company stores employee salary information on a server. Only authorized HR employees should be able to access it.

```text
Employee Data
      │
      ▼
Authentication & Access Control
      │
 ┌────┴─────┐
 ▼          ▼
Authorized  Unauthorized
   User        User
    │            │
    ▼            ▼
  Access        Denied
```

---

# ⚠️ Threats to Confidentiality

Common threats include:

Unauthorized access
Stolen passwords
Phishing
Malware and spyware
Network sniffing
Eavesdropping
Data theft
Insider threats
Weak access controls
Unencrypted communication
Lost or stolen devices

---

# 🛡️ Methods of Protecting Confidentiality

Security Control	Purpose
Authentication	Verifies the identity of users or devices.
Access Control	Restricts resources to authorized users.
Encryption	Protects data from unauthorized viewing.
Multi-Factor Authentication	Adds additional authentication protection.
Least Privilege	Gives users only the access they need.
Network Segmentation	Limits access between network areas.
Secure Protocols	Protects network communication, such as HTTPS and SSH.
Data Classification	Identifies information according to its sensitivity.

# 🌐 Confidentiality in Network Communication

Data transmitted across a network can be intercepted if it is not properly protected.

Without Encryption:

User ─────── Network ─────── Server
              │
              ▼
           Attacker
         Reads Data

With encryption:

User ─── Encrypted Data ─── Server
              │
              ▼
           Attacker
        Cannot Read Data

Encryption helps protect sensitive information while it is being transmitted.

---

# 💼 Real-World Applications

Confidentiality is important when protecting:

User passwords
Financial information
Customer information
Medical records
Employee information
Business documents
Authentication credentials
Network communications
Government information

---

# 🛠️ Skills You'll Gain

After completing this section, you'll be able to:

Define confidentiality.
Explain its role in the CIA Triad.
Identify common threats to confidentiality.
Explain how authentication and access control protect information.
Understand how encryption protects data.
Identify situations where confidentiality is important.

---

# 📌 Key Takeaways

Confidentiality ensures that information is accessible only to authorized users and systems.
It is one of the three components of the CIA Triad.
Unauthorized access, phishing, sniffing, malware, eavesdropping, and data theft can compromise confidentiality.
Authentication, access control, encryption, MFA, network segmentation, and least privilege help protect confidential information.
Encryption is especially important for protecting sensitive data during network communication.
Confidentiality is essential for protecting personal, financial, medical, business, and other sensitive information.

---

# 📚 References

- NIST Cybersecurity Framework
- NIST Special Publication 800-53 – Security and Privacy Controls
- Microsoft Learn – Security Documentation
- Cisco Networking Academy (NetAcad)
- CompTIA Security+
