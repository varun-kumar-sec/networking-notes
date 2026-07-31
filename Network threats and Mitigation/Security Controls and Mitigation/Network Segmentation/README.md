# Network Segmentation
# 📖 Overview

**Network segmentation** is the practice of dividing a network into separate logical or physical sections called **segments**.

Each segment can have its own security rules and access controls. Segmentation limits unnecessary communication between systems and helps contain security incidents.

```text
                    Internet
                       │
                       ▼
                    Firewall
                       │
          ┌────────────┼────────────┐
          ▼            ▼            ▼
       Users         Servers        IoT
      Network        Network       Network
          │            │            │
       Limited      Restricted    Restricted
       Access        Access        Access
```
---

# 🎯 Learning Objectives

After completing this section, you will be able to:

Understand network segmentation.
Explain why networks are divided into segments.
Identify common segmentation methods.
Understand VLANs and subnets.
Explain how segmentation improves security.
Understand the principle of least privilege at the network level.
Identify network segmentation best practices.

---

# 📚 Topics Covered

This section includes:

What is Network Segmentation?
Why Network Segmentation is Important
VLANs and Subnets
Network Segmentation Methods
DMZ
Microsegmentation
Network Segmentation Example
Security Benefits
Best Practices
Limitations
Real-World Applications

---

# 🌐 What is Network Segmentation?

Network segmentation divides a larger network into smaller, controlled sections.

Instead of allowing every device to communicate freely:

Without Segmentation:

PC ─── PC ─── Server ─── Printer
 │       │       │          │
 └───────┴───────┴──────────┘
     Broad Connectivity

A segmented network restricts communication:

Users ─────► User Segment
               │
               │ Limited Access
               ▼
            Servers
               │
               │ Restricted
               ▼
             Data

---

# ❓ Why Network Segmentation is Important

Segmentation helps organizations:

Reduce the attack surface.
Limit unauthorized communication.
Contain malware and security incidents.
Protect sensitive systems.
Separate different types of devices.
Apply different security policies.
Reduce lateral movement by attackers.
Improve network management.

---

# 🧩 Common Segmentation Methods

| Method                | Description                                                                                     |
| --------------------- | ----------------------------------------------------------------------------------------------- |
| **Subnetting**        | Divides a network into smaller IP networks.                                                     |
| **VLANs**             | Logically separates devices at Layer 2.                                                         |
| **Firewalls**         | Control traffic between network segments.                                                       |
| **ACLs**              | Permit or deny specific network traffic.                                                        |
| **DMZ**               | Places public-facing services in a controlled network zone.                                     |
| **Microsegmentation** | Creates highly granular security boundaries, often around individual workloads or applications. |

---

# 🔀 VLANs and Subnets
VLAN

A Virtual LAN (VLAN) logically separates devices on a switched network.

Example:

VLAN 10 → Employees
VLAN 20 → Servers
VLAN 30 → Guests
VLAN 40 → IoT Devices

Devices in different VLANs generally require a Layer 3 device, such as a router or Layer 3 switch, to communicate.

Subnet

A subnet is a logical division of an IP network.

Example:

192.168.10.0/24 → Employees
192.168.20.0/24 → Servers
192.168.30.0/24 → Guests

VLANs and subnets are related concepts but are not the same thing.

---

# 🏢 DMZ

A DMZ (Demilitarized Zone) is a network segment used to isolate services that need to be reachable from less-trusted networks, such as the Internet.

Common DMZ systems include:

Web servers
Public DNS servers
Mail gateways
Reverse proxies
Internet
    │
    ▼
 Firewall
    │
    ├────────► DMZ
    │           │
    │        Web Server
    │
    └────────► Internal Network
                │
             Databases
             User Systems

The goal is to prevent a compromise of a public-facing system from automatically providing direct access to the internal network.

---

# 🧱 Microsegmentation

Microsegmentation applies security controls at a more granular level than traditional network segmentation.

Instead of simply separating users and servers, policies can control communication between:

Individual applications
Workloads
Virtual machines
Containers
Specific services
Application A ──► Database A
      │
      ✕
      │
Application B ──► Database B

Only required communication is permitted.

---

# 💼 Network Segmentation Example

Consider a company with four types of devices:

             Firewall
                 │
     ┌───────────┼───────────┐
     ▼           ▼           ▼
  Employees    Servers      Guests
     │           │           │
     │           │           └── Internet Only
     │           │
     │           └── Restricted Access
     │
     └── Business Resources

A compromised guest device should not automatically be able to communicate with internal servers.

---

# 🔐 Security Benefits

Network segmentation can improve:

Confidentiality

Restricts access to sensitive resources.

Integrity

Limits which systems can modify or communicate with protected resources.

Availability

Can help contain malware, reduce unnecessary traffic, and limit the impact of some attacks.

Attack Containment

If one segment is compromised, security controls can limit movement into other segments.

---

# 🛡️ Network Segmentation Best Practices

Organizations should:

Identify critical systems and sensitive data.
Separate users, servers, guests, and IoT devices where appropriate.
Use VLANs and subnets appropriately.
Use firewalls or ACLs between sensitive segments.
Allow only required communication.
Apply least privilege to network access.
Monitor traffic between segments.
Regularly review segmentation rules.
Document network architecture.
Test segmentation controls.
Protect management networks separately.
Avoid relying on segmentation alone for security.

---

# ⚠️ Limitations

Network segmentation does not guarantee complete security.

Attackers may still exploit:

Misconfigured firewall rules
Compromised credentials
Vulnerable systems
Allowed network connections
Insider threats
Poorly designed segmentation

Segmentation must therefore be combined with:

Firewalls
Authentication
MFA
Endpoint protection
Encryption
Network monitoring
Patch management
Access control

---

# 🚨 Response to a Compromised Segment

If a network segment is compromised:

Identify affected systems.
Isolate the affected segment when appropriate.
Restrict communication with other segments.
Investigate logs and network traffic.
Identify the source of compromise.
Remove malware or remediate vulnerable systems.
Reset compromised credentials if necessary.
Restore affected services.
Monitor other segments for signs of lateral movement.
Review segmentation rules and improve controls.

---

# 💼 Real-World Applications

Network segmentation is commonly used in:

Corporate networks
Data centers
Cloud environments
Universities
Hospitals
Government networks
Industrial networks
IoT environments
Guest Wi-Fi networks
Multi-tenant environments

---

# 🛠️ Skills You'll Gain

After completing this section, you'll be able to:

Define network segmentation.
Explain why networks are divided into segments.
Understand VLANs and subnets.
Explain the purpose of a DMZ.
Understand microsegmentation.
Explain how firewalls and ACLs control communication between segments.
Apply the principle of least privilege at the network level.
Understand how segmentation limits lateral movement and attack impact.

---

# 📌 Key Takeaways

Network segmentation divides a network into smaller, controlled security zones.
Common techniques include subnets, VLANs, firewalls, ACLs, DMZs, and microsegmentation.
Segmentation helps reduce the attack surface and limit lateral movement.
Sensitive systems should not be unnecessarily reachable from less-trusted networks.
A DMZ can isolate public-facing services from internal systems.
Microsegmentation provides more granular communication controls.
Segmentation should follow the least-privilege principle and allow only required communication.
Network segmentation is a security layer, not a complete security solution.

---

# 📚 References

- NIST Cybersecurity Framework
- NIST SP 800-207 – Zero Trust Architecture
- CISA – Network Segmentation Guidance
- Microsoft Learn – Network Segmentation and Security
- Cisco Networking Academy (NetAcad)
- CompTIA Security+
