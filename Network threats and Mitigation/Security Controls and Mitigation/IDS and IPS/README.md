# IDS and IPS
# 📖 Overview

**Intrusion Detection Systems (IDS)** and **Intrusion Prevention Systems (IPS)** are network security controls used to identify and respond to suspicious or malicious activity.

An **IDS** primarily detects and alerts on potential threats, while an **IPS** can detect and automatically take action to block or prevent certain threats.

```text
                Network Traffic
                       │
                       ▼
                  IDS / IPS
                       │
             ┌─────────┴─────────┐
             ▼                   ▼
          Detect              Analyze
             │                   │
             ▼                   ▼
           Alert             Take Action
                               │
                          IPS: Block
```
---

# 🎯 Learning Objectives

After completing this section, you will be able to:

Understand IDS and IPS.
Differentiate between IDS and IPS.
Identify common detection methods.
Understand network-based and host-based IDS/IPS.
Explain how IDS/IPS works with firewalls.
Identify basic IDS/IPS deployment and security practices.

---

# 📚 Topics Covered

This section includes:

What is IDS?
What is IPS?
IDS vs IPS
Detection Methods
Network-Based and Host-Based Systems
How IDS/IPS Works
IDS/IPS and Firewalls
False Positives and False Negatives
Deployment Considerations
Best Practices
Real-World Applications

---

# 🔍 What is IDS?

An Intrusion Detection System (IDS) monitors network or system activity for signs of suspicious or malicious behavior.

When a potential threat is detected, an IDS typically:

Generates an alert.
Records relevant information.
Sends information to monitoring or security systems.
Helps security teams investigate the event.
Network Traffic
      │
      ▼
     IDS
      │
      ▼
Traffic Analysis
      │
      ▼
Suspicious Activity
      │
      ▼
     Alert

An IDS generally does not automatically block the traffic it detects.

---

# 🛡️ What is IPS?

An Intrusion Prevention System (IPS) monitors traffic and can automatically take action against detected malicious activity.

Possible actions include:

Blocking traffic
Dropping packets
Resetting connections
Blocking malicious sources
Generating alerts
Logging security events
Network Traffic
      │
      ▼
     IPS
      │
      ▼
Traffic Analysis
      │
 ┌────┴────┐
 ▼         ▼
Normal   Malicious
 │          │
 ▼          ▼
Allow      Block

---

# ⚖️ IDS vs IPS

| IDS                                                       | IPS                                                       |
| --------------------------------------------------------- | --------------------------------------------------------- |
| Detects suspicious activity.                              | Detects and can prevent suspicious activity.              |
| Primarily generates alerts.                               | Can automatically block or modify traffic.                |
| Usually operates out-of-band.                             | Commonly deployed inline.                                 |
| Lower risk of accidentally disrupting legitimate traffic. | Incorrect rules can potentially block legitimate traffic. |
| Useful for monitoring and investigation.                  | Useful for real-time prevention.                          |

---

# 🧠 Detection Methods

IDS and IPS can use different methods to identify threats.

| Method                        | Description                                                    |
| ----------------------------- | -------------------------------------------------------------- |
| **Signature-Based Detection** | Looks for known patterns associated with known attacks.        |
| **Anomaly-Based Detection**   | Identifies activity that differs from an established baseline. |
| **Behavior-Based Detection**  | Looks for suspicious behaviors or activity patterns.           |
| **Rule-Based Detection**      | Uses predefined security rules to identify specific events.    |

Signature-Based Example
Known Attack Pattern
        │
        ▼
IDS / IPS Signature
        │
        ▼
Pattern Match
        │
        ▼
Alert / Block

Signature-based detection is effective for known threats but may have difficulty identifying completely new attack patterns.

---

# 🌐 Network-Based vs Host-Based
Network-Based IDS/IPS (NIDS/NIPS)

Monitors network traffic moving through a network segment.

Internet
   │
   ▼
Network
   │
   ▼
NIDS / NIPS
   │
   ▼
Internal Systems
Host-Based IDS/IPS (HIDS/HIPS)

Monitors activity on an individual computer or server.

It may monitor:

System files
Processes
Logs
User activity
Network connections
Configuration changes
Computer
   │
   ├── Processes
   ├── Files
   ├── Logs
   └── Network Activity
            │
            ▼
           HIDS

---

# 🔄 How IDS/IPS Works

A simplified process is:

Traffic or system activity is collected.
The system analyzes the activity.
Detection rules or models are applied.
Suspicious activity is identified.
An IDS generates an alert.
An IPS may automatically block or prevent the activity.
Events are logged for investigation.
Traffic
   ↓
Collection
   ↓
Analysis
   ↓
Detection
   ↓
┌───────────────┐
│ IDS → Alert   │
│ IPS → Block   │
└───────────────┘
   ↓
Logging / Investigation

---

# 🧱 IDS/IPS and Firewalls

IDS/IPS and firewalls have different but complementary roles.
| Firewall                                                   | IDS/IPS                                                |
| ---------------------------------------------------------- | ------------------------------------------------------ |
| Controls traffic based on security rules.                  | Detects suspicious or malicious activity.              |
| Commonly controls IPs, ports, protocols, and applications. | Can identify attack patterns and suspicious behavior.  |
| Decides whether traffic should be permitted.               | Provides detection and, for IPS, automated prevention. |

Internet
   │
   ▼
Firewall
   │
   ▼
IDS / IPS
   │
   ▼
Internal Network

Modern security platforms may combine firewall, IDS/IPS, and other security capabilities into a single system.

---

# ⚠️ False Positives and False Negatives

False Positive

The system identifies legitimate activity as malicious.

Normal Traffic
     │
     ▼
Detected as Attack
     │
     ▼
False Positive

Too many false positives can create alert fatigue and may cause legitimate traffic to be blocked by an IPS.

False Negative

The system fails to detect actual malicious activity.

Malicious Traffic
     │
     ▼
Not Detected
     │
     ▼
False Negative

False negatives are particularly dangerous because an attack may continue unnoticed.

---

# 🛠️ Deployment Considerations

When deploying IDS/IPS, organizations should consider:

Network architecture
Traffic volume
Critical systems
Network segments
Required visibility
Performance requirements
Alert volume
False-positive rates
Placement of sensors
Integration with security monitoring systems

IPS systems should be carefully tested before enabling aggressive blocking rules.

---

# 🛡️ IDS/IPS Best Practices

Organizations should:

Keep detection signatures updated.
Monitor and investigate alerts.
Tune rules to reduce false positives.
Protect IDS/IPS management interfaces.
Keep the system updated.
Integrate alerts with centralized monitoring where appropriate.
Review detection rules regularly.
Test IPS blocking policies carefully.
Monitor system performance.
Combine IDS/IPS with firewalls, endpoint protection, MFA, and network segmentation.

---

# 🚨 Responding to an IDS/IPS Alert

When a significant alert occurs:

Review the alert details.
Identify affected systems.
Determine whether the activity is legitimate or malicious.
Review related network and system logs.
Contain the threat when necessary.
Investigate the source and impact.
Remediate affected systems.
Update security rules if necessary.
Document the incident.
Alert
  │
  ▼
Validate
  │
  ▼
Investigate
  │
  ▼
Contain
  │
  ▼
Remediate
  │
  ▼
Improve Detection

---

# 🔐 IDS/IPS and the CIA Triad

| CIA Objective       | IDS/IPS Contribution                                                   |
| ------------------- | ---------------------------------------------------------------------- |
| **Confidentiality** | Helps detect or block attacks that could expose sensitive information. |
| **Integrity**       | Helps identify malicious activity that could modify systems or data.   |
| **Availability**    | IPS can block certain attacks that could disrupt services.             |

---

# 💼 Real-World Applications

IDS and IPS are commonly used in:

Corporate networks
Data centers
Cloud environments
Government networks
Financial institutions
Healthcare organizations
Educational institutions
Internet gateways
Critical infrastructure

---

# 🛠️ Skills You'll Gain

After completing this section, you'll be able to:

Define IDS and IPS.
Explain the difference between detection and prevention.
Understand signature-based and anomaly-based detection.
Differentiate between network-based and host-based systems.
Explain how IDS/IPS works with firewalls.
Understand false positives and false negatives.
Identify basic IDS/IPS deployment and monitoring practices.
Understand how to respond to IDS/IPS alerts.

---

# 📌 Key Takeaways

IDS primarily detects suspicious activity and generates alerts.
IPS can detect suspicious activity and automatically take preventive action.
Detection methods include signature-based, anomaly-based, behavior-based, and rule-based detection.
NIDS/NIPS monitor network activity, while HIDS/HIPS monitor individual hosts.
IDS/IPS and firewalls perform different but complementary security functions.
False positives identify legitimate activity as malicious, while false negatives fail to detect real threats.
IDS/IPS systems require regular updates, monitoring, tuning, and testing.
IPS blocking rules should be carefully configured to avoid disrupting legitimate traffic.
IDS/IPS is one layer of defense and should be combined with other controls such as firewalls, endpoint protection, MFA, segmentation, patching, and backups.

---

# 📚 References

- NIST Cybersecurity Framework
- NIST SP 800-94 – Guide to Intrusion Detection and Prevention Systems
- CISA – Intrusion Detection and Prevention Guidance
- Microsoft Learn – Security and Network Monitoring
- Cisco Networking Academy (NetAcad)
- CompTIA Security+
