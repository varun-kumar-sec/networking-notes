# Network Sniffing
# 📖 Overview

**Network sniffing** is the process of capturing and analyzing network packets as they travel across a network. It can be used legitimately for **network troubleshooting and security monitoring**, but attackers can also use it to intercept sensitive information.

Sniffing becomes a security threat when an unauthorized person captures or analyzes network traffic to obtain information such as credentials, session data, or other sensitive information.

---

# 🎯 Learning Objectives

After completing this section, you will be able to:

- Understand what network sniffing is.
- Explain how packet capture works.
- Differentiate between legitimate and malicious sniffing.
- Identify passive and active sniffing.
- Understand the risks of network sniffing.
- Identify methods used to protect network traffic.

---

# 📚 Topics Covered

This section includes:

- What is Network Sniffing?
- Packet Capture
- Passive and Active Sniffing
- Legitimate Uses
- Malicious Uses
- Network Sniffing Examples
- Effects on the CIA Triad
- Sniffing Prevention and Mitigation
- Real-World Applications

---

# 🌐 What is Network Sniffing?

Network sniffing involves capturing network packets and examining their contents or metadata.

```text
Device A
   │
   │ Network Packets
   ▼
Network ───────────► Device B
   │
   ▼
Packet Capture
   │
   ▼
Packet Analysis
```
A packet analyzer can display information such as:

Source and destination addresses
Protocols
Ports
Packet contents, when available
Timing and traffic patterns

Modern encrypted protocols such as HTTPS and SSH protect the contents of communications, although some traffic metadata may still be observable.

---

# 🔍 Passive vs Active Sniffing

| Type                 | Description                                                                                                  |
| -------------------- | ------------------------------------------------------------------------------------------------------------ |
| **Passive Sniffing** | Captures traffic without actively interfering with the communication.                                        |
| **Active Sniffing**  | Involves manipulating or influencing network traffic to capture traffic that would otherwise not be visible. |

Passive sniffing is more commonly associated with shared or broadcast network environments, while active techniques may be used against switched networks.

---

# 🛠️ Legitimate Uses

Network administrators and security professionals use packet analysis for:

Troubleshooting connectivity problems
Diagnosing network performance issues
Investigating security incidents
Monitoring protocols
Detecting unusual traffic
Verifying network configurations
Analyzing application communication

Common packet-analysis tools include Wireshark and tcpdump.

Packet capture should only be performed on networks and systems where you have appropriate authorization.

---

# ⚠️ Malicious Uses

Attackers may use network sniffing to attempt to:

Capture credentials sent without encryption
Intercept sensitive information
Collect session information
Analyze network traffic patterns
Identify devices and services
Support Man-in-the-Middle attacks
Unencrypted Traffic
       │
       ▼
Packet Capture
       │
       ▼
Sensitive Information
       │
       ▼
Potential Data Theft

---

# 💼 Network Sniffing Example

Consider a user accessing a service using an insecure, unencrypted protocol.

User ───────► Network ───────► Server
                 │
                 ▼
             Sniffer
                 │
                 ▼
          Captures Traffic

If sensitive information is transmitted without adequate protection, the captured traffic may expose that information.

With encrypted communication:

User ──► Encrypted Traffic ──► Server
                 │
                 ▼
              Sniffer
                 │
                 ▼
        Cannot Easily Read
        Protected Contents

---

# 🔐 Effects on the CIA Triad

Network sniffing can primarily affect:
| CIA Objective       | Possible Effect                                                                  |
| ------------------- | -------------------------------------------------------------------------------- |
| **Confidentiality** | Sensitive information may be intercepted.                                        |
| **Integrity**       | Active interception techniques may allow traffic manipulation.                   |
| **Availability**    | Usually not the primary objective, although active attacks can cause disruption. |

---

# 🛡️ Sniffing Prevention and Mitigation

Organizations can reduce sniffing risks by:

Using HTTPS/TLS for web communication.
Using SSH instead of insecure remote-access protocols.
Using secure Wi-Fi encryption such as WPA2 or WPA3.
Using VPNs when appropriate.
Avoiding untrusted public networks for sensitive activities.
Using network segmentation.
Configuring switches securely.
Monitoring unusual network activity.
Applying strong authentication and MFA.
Keeping network devices and systems updated.

---

# 🚨 Response to Suspicious Sniffing

If unauthorized packet capture is suspected:

Identify affected systems and network segments.
Review network and security logs.
Check for unauthorized devices or access points.
Investigate unusual network traffic.
Change potentially exposed credentials.
Revoke compromised sessions when appropriate.
Report the incident to the IT/security team.
Improve network encryption and access controls.

---

# 💼 Real-World Applications

Network sniffing and packet analysis are used in:

Network troubleshooting
Security operations
Incident response
Network monitoring
Protocol analysis
Performance analysis
Penetration testing with authorization
Digital forensics

---

# 🛠️ Skills You'll Gain

After completing this section, you'll be able to:

Define network sniffing.
Explain how packets are captured and analyzed.
Differentiate between passive and active sniffing.
Identify legitimate and malicious uses of packet capture.
Understand how sniffing can threaten confidentiality.
Explain how encryption and secure protocols reduce sniffing risks.
Understand basic steps for investigating suspicious packet capture.

---

# 📌 Key Takeaways

Network sniffing involves capturing and analyzing network packets.
It can be a legitimate tool for troubleshooting, monitoring, and security analysis.
Unauthorized sniffing can be used to intercept sensitive information.
Passive sniffing observes traffic, while active sniffing involves manipulating or influencing traffic.
Unencrypted protocols are particularly vulnerable to information exposure.
HTTPS/TLS, SSH, secure Wi-Fi, VPNs, network segmentation, strong authentication, and monitoring help reduce sniffing risks.
Packet capture should only be performed on networks where you have appropriate authorization.

---

# 📚 References

- NIST Cybersecurity Framework
- CISA – Network Security Guidance
- Wireshark Documentation
- Microsoft Learn – Network Security Documentation
- Cisco Networking Academy (NetAcad)
- CompTIA Security+
