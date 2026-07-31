# Man-in-the-Middle (MitM) Attack
# 📖 Overview

A **Man-in-the-Middle (MitM) attack** occurs when an attacker secretly positions themselves between two communicating parties and intercepts, relays, or potentially modifies their communication without the parties realizing it.

MitM attacks can affect **confidentiality** and **integrity**, and in some cases can also lead to unauthorized access.

---

# 🎯 Learning Objectives

After completing this section, you will be able to:

- Understand what a MitM attack is.
- Explain how MitM attacks work.
- Identify common MitM techniques.
- Understand the risks caused by MitM attacks.
- Identify methods used to prevent MitM attacks.

---

# 📚 Topics Covered

This section includes:

- What is a MitM Attack?
- How MitM Attacks Work
- Common MitM Techniques
- MitM Attack Examples
- Effects on the CIA Triad
- MitM Prevention and Mitigation
- Real-World Applications

---

# 🔐 What is a MitM Attack?

In a MitM attack, the attacker attempts to place themselves between two communicating parties.

```text
Normal Communication:

User ───────────────► Server
       Direct Connection


MitM Communication:

User ─────► Attacker ─────► Server
              │
              ▼
        Intercept / Relay
        / Potentially Modify
```
The attacker may attempt to:

Read sensitive information.
Capture credentials.
Monitor communications.
Modify data.
Redirect traffic.
Impersonate one of the communicating parties.

---

# 🔄 How MitM Attacks Work

A simplified MitM attack can involve:

Positioning – The attacker gains a position between communicating systems.
Interception – Network traffic is intercepted.
Relay – The attacker forwards traffic so communication appears normal.
Inspection or Modification – The attacker may read or alter information.
Data Collection – Sensitive information may be captured.
User
 │
 │ Request
 ▼
Attacker
 │
 │ Forwarded Request
 ▼
Server
 │
 │ Response
 ▼
Attacker
 │
 │ Forwarded Response
 ▼
User

---

# 🧩 Common MitM Techniques

| Technique                    | Description                                                               |
| ---------------------------- | ------------------------------------------------------------------------- |
| **Rogue Wi-Fi Access Point** | Attacker creates a malicious wireless network that users connect to.      |
| **ARP Spoofing**             | Attacker sends forged ARP information to influence local network traffic. |
| **DNS Spoofing**             | Attempts to provide false DNS responses and redirect users.               |
| **Session Hijacking**        | Attempts to take control of an authenticated session.                     |
| **SSL/TLS Downgrade**        | Attempts to force communication toward weaker or less secure protection.  |
| **Evil Twin**                | A fraudulent Wi-Fi access point impersonates a legitimate network.        |

---

# 💼 MitM Example

A user connects to an unsecured or malicious Wi-Fi network.

User
  │
  ▼
Fake Wi-Fi Access Point
  │
  ▼
Attacker
  │
  ▼
Internet

If communication is not properly protected, the attacker may be able to observe or manipulate traffic.

Using properly configured HTTPS/TLS helps protect application data even when network traffic is intercepted.

---

# ⚠️ Effects of MitM Attacks

A successful MitM attack can result in:

Credential theft
Data interception
Session compromise
Unauthorized transactions
Data modification
Privacy violations
Redirection to malicious websites

MitM attacks can therefore affect:
| CIA Objective   | Possible Effect                                         |
| --------------- | ------------------------------------------------------- |
| Confidentiality | Sensitive data may be intercepted.                      |
| Integrity       | Data may be modified in transit.                        |
| Availability    | Usually not the primary goal, but disruption may occur. |

---

# 🛡️ MitM Prevention and Mitigation

Organizations and users can reduce MitM risks by:

Using HTTPS/TLS for web communication.
Using secure protocols such as SSH instead of insecure remote-access protocols.
Avoiding untrusted or suspicious Wi-Fi networks.
Using properly secured Wi-Fi encryption.
Using VPNs when appropriate.
Verifying certificates and security warnings.
Keeping operating systems and network devices updated.
Using strong authentication and MFA.
Implementing network segmentation.
Monitoring unusual network activity.
Using secure DNS mechanisms where appropriate.

Important: A VPN can protect traffic between the device and the VPN endpoint, but it does not make every endpoint or application automatically trustworthy.

---

# 🚨 Response to a Suspected MitM Attack

If a MitM attack is suspected:

Disconnect from the suspicious network.
Use a trusted network.
Check for certificate or browser security warnings.
Change potentially compromised credentials.
Revoke active sessions when appropriate.
Report the incident to the responsible IT/security team.
Review network and system logs when available.
Investigate potentially compromised devices or accounts.

---

# 💼 Real-World Applications

MitM protection is important when using:

Public Wi-Fi
Corporate networks
Online banking
Cloud services
Remote-access systems
Web applications
Email services
Wireless networks

---

# 🛠️ Skills You'll Gain

After completing this section, you'll be able to:

Define a Man-in-the-Middle attack.
Explain how MitM attacks work.
Identify common MitM techniques.
Understand how MitM attacks affect confidentiality and integrity.
Explain the role of HTTPS/TLS, VPNs, secure protocols, and certificate validation.
Identify basic steps for responding to a suspected MitM attack.

---

# 📌 Key Takeaways

A MitM attack occurs when an attacker intercepts communication between two parties.
The attacker may read, relay, modify, or redirect network traffic.
Common techniques include rogue Wi-Fi, ARP spoofing, DNS spoofing, session hijacking, Evil Twin attacks, and TLS downgrade attempts.
MitM attacks primarily threaten Confidentiality and Integrity.
HTTPS/TLS, secure Wi-Fi, VPNs, certificate validation, MFA, patching, and network monitoring help reduce MitM risks.
Users should avoid untrusted networks and never ignore unexpected security or certificate warnings.
A VPN protects the connection to its endpoint, but secure application protocols and trusted endpoints are still necessary.

---

# 📚 References

- NIST Cybersecurity Framework
- CISA – Network Security Guidance
- Microsoft Learn – Network Security Documentation
- Cisco Networking Academy (NetAcad)
- CompTIA Security+
