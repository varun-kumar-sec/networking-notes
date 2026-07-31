# Availability

> **Module:** Network Threats and Mitigation  
> **Section:** CIA Triad – Availability  
> **Difficulty:** Beginner  
> **Prerequisites:** Network Security, Confidentiality, Integrity  
> **Estimated Reading Time:** 5–7 Minutes

---

# 📖 Overview

**Availability** is the security principle of ensuring that systems, networks, applications, and data are **accessible and usable by authorized users when needed**.

Availability is one of the three components of the **CIA Triad**, along with Confidentiality and Integrity.

---

# 🎯 Learning Objectives

After completing this section, you will be able to:

- Understand what availability means.
- Explain why availability is important in network security.
- Identify common threats to availability.
- Identify methods used to maintain availability.
- Understand the importance of redundancy, backups, and disaster recovery.

---

# 📚 Topics Covered

This section includes:

- What is Availability?
- Importance of Availability
- Threats to Availability
- Methods of Maintaining Availability
- High Availability and Redundancy
- Backup and Disaster Recovery
- Real-World Applications

---

# 🌐 What is Availability?

Availability ensures that authorized users can access required systems, services, applications, and data when they need them.

For example, an organization's employees should be able to access its file server during working hours.

```text
Authorized User
      │
      ▼
   Network
      │
      ▼
Available Server
      │
      ▼
   Access Granted

```
---

# ⚠️ Threats to Availability

Common threats include:

Denial-of-Service (DoS) attacks
Distributed Denial-of-Service (DDoS) attacks
Malware and ransomware
Hardware failure
Power failure
Network outages
Software failures
Misconfiguration
Natural disasters
Physical damage
Resource exhaustion

---

# 🛡️ Methods of Maintaining Availability

Security/Recovery Control	Purpose
Redundancy	Provides alternative components when one fails.
Backups	Allows data to be restored after loss or damage.
Failover	Automatically switches to another system when a primary system fails.
Load Balancing	Distributes traffic across multiple systems.
UPS	Provides temporary power during electrical failures.
Disaster Recovery	Provides procedures for restoring services after major incidents.
Monitoring	Detects failures and availability problems.
Regular Maintenance	Reduces failures caused by outdated or damaged systems.
DDoS Protection	Helps reduce the impact of denial-of-service attacks.

---

# 🔄 High Availability and Redundancy

High availability (HA) means designing systems to remain operational with minimal downtime.

Redundancy means having additional components or systems available if the primary component fails.

Example:

              Network Traffic
                    │
          ┌─────────┴─────────┐
          ▼                   ▼
      Server 1             Server 2
     (Primary)            (Backup)
          │                   │
          └─────────┬─────────┘
                    ▼
               High Availability

If one server fails, another server can continue providing the service.

---

# 💾 Backup and Disaster Recovery

Backups protect against data loss caused by:

Ransomware
Hardware failure
Accidental deletion
System corruption
Security incidents

Disaster recovery focuses on restoring systems and services after a major disruption.

A good recovery strategy should consider:

What data needs to be backed up.
How frequently backups should occur.
Where backups are stored.
How quickly systems need to be restored.
How backups will be tested.

---

# 📊 Availability Concepts

Two important measurements are:

Uptime

The amount of time a system remains operational and accessible.

Downtime

The amount of time a system or service is unavailable.

Organizations often define availability requirements using Service Level Agreements (SLAs).

---

# 💼 Real-World Applications

Availability is important for:

Online banking
E-commerce websites
Cloud services
Healthcare systems
Government services
Corporate networks
DNS and network services
Email systems
Data centers
Emergency services

Even a short outage can result in financial loss, productivity loss, or disruption of critical services.

---

# 🛠️ Skills You'll Gain

After completing this section, you'll be able to:

Define availability.
Explain its role in the CIA Triad.
Identify threats that can cause service disruption.
Explain redundancy and high availability.
Understand the purpose of backups and disaster recovery.
Explain the role of monitoring and failover.
Recognize situations where availability is critical.

---

# 📌 Key Takeaways

Availability ensures that authorized users can access systems, services, and data when needed.
It is one of the three components of the CIA Triad.
DoS/DDoS attacks, hardware failures, malware, power outages, misconfigurations, and disasters can affect availability.
Redundancy, failover, load balancing, backups, monitoring, UPS systems, and disaster recovery help maintain availability.
High availability reduces downtime by using redundant systems or components.
Backups help restore lost data, while disaster recovery focuses on restoring systems and services.
Availability is especially important for critical services such as banking, healthcare, cloud platforms, and corporate networks.

---

# 📚 References

NIST Cybersecurity Framework
NIST Special Publication 800-34 – Contingency Planning Guide
Microsoft Learn – Security Documentation
Cisco Networking Academy (NetAcad)
CompTIA Security+
