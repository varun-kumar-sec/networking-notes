# Integrity
# 📖 Overview

**Integrity** is the security principle of ensuring that information remains **accurate, complete, consistent, and protected from unauthorized modification or destruction**.

Integrity is one of the three components of the **CIA Triad**, along with Confidentiality and Availability.

---

# 🎯 Learning Objectives

After completing this section, you will be able to:

- Understand what integrity means.
- Explain why integrity is important in network security.
- Identify common threats to data integrity.
- Identify methods used to protect integrity.
- Understand the role of hashing, access control, and digital signatures.

---

# 📚 Topics Covered

This section includes:

- What is Integrity?
- Importance of Integrity
- Threats to Integrity
- Methods of Protecting Integrity
- Data Integrity in Network Communication
- Real-World Applications

---

# 🔐 What is Integrity?

Integrity ensures that information is not **altered, deleted, or corrupted without authorization**.

For example, if a company's financial record shows a payment of `$1,000`, an attacker should not be able to change it to `$10,000` without authorization.

```text
Original Data
     │
     ▼
Security Controls
     │
     ▼
Authorized Changes ──► Allowed
Unauthorized Changes ─► Blocked/Detected
```
---

# ⚠️ Threats to Integrity

Common threats include:

Unauthorized modification
Malware
Data corruption
Man-in-the-Middle attacks
Compromised user accounts
Insider threats
Incorrect configuration
Software vulnerabilities
File tampering
Database manipulation

---

# 🛡️ Methods of Protecting Integrity

Security Control	Purpose
Access Control	Prevents unauthorized users from modifying data.
Hashing	Detects whether data has been changed.
Digital Signatures	Verifies data authenticity and detects modification.
File Permissions	Controls who can modify files and folders.
Backups	Allows recovery of correct data after corruption or tampering.
Encryption	Protects data from unauthorized modification during transmission when properly implemented.
Version Control	Tracks changes and allows previous versions to be restored.
Monitoring	Detects suspicious or unauthorized changes.

---

# #️⃣ Hashing and Integrity

A hash function generates a fixed-length value from data.

If the original data changes, its hash will normally change as well.

Original File
     │
     ▼
Hash Function
     │
     ▼
Hash Value

Later, the file can be hashed again and the values compared.

Original Hash ──────┐
                    ├──► Compare
New Hash ───────────┘
                       │
              ┌────────┴────────┐
              ▼                 ▼
           Same              Different
        No detected          Data may
          change             have changed

Common cryptographic hash algorithms include SHA-256 and SHA-3.

Note: Hashing is generally used to verify integrity; it is not encryption and is not designed to recover the original data.

---

# ✍️ Digital Signatures

A digital signature helps verify:

Who signed the data.
Whether the data was modified after signing.

Digital signatures use public-key cryptography and cryptographic hashes.

They are commonly used with:

Software
Documents
Certificates
Secure communications

---

# 🌐 Integrity in Network Communication

Data transmitted across a network can be modified if communication is not properly protected.

Sender
   │
   ▼
Data + Integrity Protection
   │
   ▼
Network
   │
   ▼
Receiver
   │
   ▼
Verify Data

Secure protocols and cryptographic mechanisms can help detect or prevent unauthorized modification.

---

# 💼 Real-World Applications

Integrity is important when protecting:

Financial transactions
Database records
Software packages
Operating system files
Network configurations
Medical records
Business documents
Authentication information
Network communications

---

# 🛠️ Skills You'll Gain

After completing this section, you'll be able to:

Define integrity.
Explain its role in the CIA Triad.
Identify threats that can compromise data integrity.
Explain how access control protects data from unauthorized modification.
Understand how hashing helps verify data integrity.
Understand the purpose of digital signatures.
Recognize situations where integrity is critical.

---

# 📌 Key Takeaways

Integrity ensures that information remains accurate, complete, and protected from unauthorized modification.
It is one of the three components of the CIA Triad.
Malware, unauthorized access, data corruption, insider threats, and tampering can compromise integrity.
Access control, file permissions, hashing, digital signatures, backups, monitoring, and version control help protect integrity.
A changed file normally produces a different cryptographic hash.
Hashing is used for integrity verification, not encryption.
Digital signatures help verify the authenticity and integrity of digitally signed information.
Maintaining integrity is critical for financial records, databases, software, configurations, and other important information.

---

# 📚 References

NIST Cybersecurity Framework
NIST Special Publication 800-57 – Recommendation for Key Management
Microsoft Learn – Security Documentation
Cisco Networking Academy (NetAcad)
CompTIA Security+
