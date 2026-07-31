# Denial of Service (DoS)
# 📖 Overview

**Denial of Service (DoS)** is an attack that attempts to make a system, server, application, or network service **unavailable to legitimate users**.

A DoS attack typically overwhelms or exhausts the target's resources, such as bandwidth, processing power, memory, or connection capacity.

A **Distributed Denial of Service (DDoS)** attack uses multiple systems or devices to generate traffic or requests toward the target.

---

# 🎯 Learning Objectives

After completing this section, you will be able to:

- Understand what a DoS attack is.
- Differentiate between DoS and DDoS.
- Identify common types of DoS attacks.
- Understand the impact of DoS attacks.
- Identify methods used to prevent and mitigate DoS attacks.

---

# 📚 Topics Covered

This section includes:

- What is Denial of Service?
- DoS vs DDoS
- How DoS Attacks Work
- Types of DoS Attacks
- Common Effects
- DoS/DDoS Mitigation
- Real-World Applications

---

# 🚫 What is Denial of Service?

A DoS attack attempts to prevent legitimate users from accessing a service.

```text
Attacker
   │
   ▼
Large Number of Requests
   │
   ▼
Target Server
   │
   ▼
Resources Exhausted
   │
   ▼
Service Becomes Unavailable
```
The primary security objective affected by DoS attacks is Availability.

---

# 🌐 DoS vs DDoS

| DoS                                                               | DDoS                                                                     |
| ----------------------------------------------------------------- | ------------------------------------------------------------------------ |
| Usually originates from one attacking system or a limited source. | Uses many distributed systems or devices.                                |
| Smaller attack infrastructure.                                    | Larger and more distributed attack infrastructure.                       |
| Can be easier to identify and block in some cases.                | Can be more difficult to filter because traffic comes from many sources. |

A DDoS attack may use a botnet, which is a collection of compromised devices controlled by an attacker.

---

# 🧩 Types of DoS Attacks

| Type                         | Description                                                                 |
| ---------------------------- | --------------------------------------------------------------------------- |
| **Volumetric Attack**        | Attempts to overwhelm available network bandwidth.                          |
| **Protocol Attack**          | Exploits weaknesses in network or transport protocols to consume resources. |
| **Application-Layer Attack** | Overwhelms a specific application or service with requests.                 |
| **Resource Exhaustion**      | Consumes CPU, memory, connection tables, or other system resources.         |

---

# ⚠️ Common Effects

A successful DoS/DDoS attack can cause:

Website unavailability
Slow network performance
Application failure
Server resource exhaustion
Loss of productivity
Financial losses
Service interruptions
Damage to an organization's reputation

---

# 💼 Simple Example

Normal Traffic
      │
      ▼
┌──────────────┐
│    Server    │
└──────────────┘
      │
      ▼
Service Available

During an attack:

Attack Traffic
   ↓ ↓ ↓ ↓ ↓
   ↓ ↓ ↓ ↓ ↓
┌──────────────┐
│    Server    │
└──────────────┘
      │
      ▼
Resources Exhausted
      │
      ▼
Service Unavailable

---

# 🛡️ DoS/DDoS Mitigation

Organizations can reduce the impact of DoS/DDoS attacks by using:

Firewalls
Rate limiting
Traffic filtering
IDS/IPS
Load balancing
Network segmentation
DDoS protection services
Content Delivery Networks (CDNs)
Redundant infrastructure
Continuous network monitoring
Incident response procedures

A layered approach is usually more effective than relying on a single control.

---

# 🚨 Response to a DoS/DDoS Attack

When an attack is detected:

Identify abnormal traffic patterns.
Determine the affected services.
Apply filtering or rate-limiting controls.
Redirect traffic to mitigation infrastructure when available.
Monitor system and network performance.
Preserve relevant logs and evidence.
Restore normal service after the attack.
Review the incident and improve defenses.

---

# 💼 Real-World Applications

DoS/DDoS protection is important for:

Websites
Online stores
Banking services
Cloud applications
DNS services
Gaming platforms
Corporate networks
Government services
Critical online infrastructure

---

# 🛠️ Skills You'll Gain

After completing this section, you'll be able to:

Define a DoS attack.
Explain the difference between DoS and DDoS.
Identify common DoS attack categories.
Explain how DoS attacks affect availability.
Identify common effects of DoS attacks.
Explain basic DoS/DDoS mitigation techniques.
Understand basic incident response steps.

---

# 📌 Key Takeaways

DoS attacks attempt to make systems or services unavailable to legitimate users.
DDoS attacks use multiple distributed systems or devices.
DoS attacks primarily target Availability in the CIA Triad.
Attacks can exhaust bandwidth, CPU, memory, connection capacity, or application resources.
Common categories include volumetric, protocol, application-layer, and resource-exhaustion attacks.
Rate limiting, filtering, firewalls, IDS/IPS, load balancing, CDNs, DDoS protection, monitoring, and redundancy help reduce the impact.
Effective protection uses multiple layers of security rather than a single control.

---

# 📚 References

- NIST Cybersecurity Framework
- CISA – Denial-of-Service Guidance
- Microsoft Learn – Network Security Documentation
- Cisco Networking Academy (NetAcad)
- CompTIA Security+
