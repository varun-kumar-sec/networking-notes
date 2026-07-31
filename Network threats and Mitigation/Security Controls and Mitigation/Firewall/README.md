# Firewall
# 📖 Overview

A **firewall** is a security device or software that **monitors and controls network traffic** based on predefined security rules.

Firewalls are commonly placed between trusted and untrusted networks, such as between an organization's internal network and the Internet.

```text
Internet
   │
   ▼
┌──────────────┐
│   Firewall   │
│ Security     │
│    Rules     │
└──────────────┘
   │
   ▼
Internal Network
```
A firewall can help prevent unauthorized network connections while allowing legitimate traffic.

---

# 🎯 Learning Objectives

After completing this section, you will be able to:

Understand what a firewall is.
Explain how firewalls control network traffic.
Identify common types of firewalls.
Understand firewall rules.
Explain the role of firewalls in network security.
Identify basic firewall configuration and security practices.

---

# 📚 Topics Covered

This section includes:

What is a Firewall?
How a Firewall Works
Firewall Rules
Types of Firewalls
Stateful and Stateless Firewalls
Host-Based and Network-Based Firewalls
Firewall Examples
Firewall Security Best Practices
Limitations of Firewalls
Real-World Applications

---

# 🛡️ What is a Firewall?

A firewall acts as a traffic-control point between networks or systems.

It examines network traffic and applies configured rules to determine whether traffic should be:

Allowed
Blocked
Rejected
Logged
Incoming Traffic
       │
       ▼
   Firewall
       │
   ┌───┴───┐
   ▼       ▼
 Allowed  Blocked
   │
   ▼
Internal Resource

---

# 🔄 How a Firewall Works

A simplified process is:

Network traffic reaches the firewall.
The firewall examines relevant traffic information.
It compares the traffic against security rules.
The firewall takes the configured action.
The event may be logged for monitoring.

Firewalls can consider information such as:

Source IP address
Destination IP address
Source and destination ports
Network protocol
Connection state
Application information, depending on firewall type

---

# 📜 Firewall Rules

Firewall rules define what traffic is permitted or denied.

Example:
| Source           | Destination            | Protocol | Port | Action |
| ---------------- | ---------------------- | -------- | ---- | ------ |
| Any              | Web Server             | TCP      | 443  | Allow  |
| Any              | Internal Admin Service | TCP      | 3389 | Deny*  |
| Internal Network | DNS Server             | UDP/TCP  | 53   | Allow  |
| Any              | Any                    | Any      | Any  | Deny*  |
*Rules depend on the organization's requirements and should be configured carefully.

A common security principle is:

Allow only the traffic that is required and deny unnecessary traffic.

---

# 🧩 Types of Firewalls

| Type                                | Description                                                                                                                      |
| ----------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| **Packet-Filtering Firewall**       | Filters traffic based on information such as IP addresses, ports, and protocols.                                                 |
| **Stateful Firewall**               | Tracks connection state and makes decisions based on the context of connections.                                                 |
| **Proxy Firewall**                  | Acts as an intermediary between clients and servers.                                                                             |
| **Next-Generation Firewall (NGFW)** | Provides advanced inspection and security features, often including application awareness and intrusion-prevention capabilities. |
| **Host-Based Firewall**             | Runs directly on an individual computer or server.                                                                               |
| **Network-Based Firewall**          | Protects multiple systems by controlling traffic between networks.                                                               |

---

# 🔗 Stateful vs Stateless
Stateless Firewall

Examines each packet primarily according to configured rules without maintaining connection state.

Stateful Firewall

Maintains information about active connections and can make decisions based on whether traffic belongs to an expected connection.

Stateless:
Packet → Rule Check → Allow/Deny

Stateful:
Connection → State Tracking → Rule Check → Allow/Deny

---

# 💻 Host-Based vs Network-Based
Host-Based Firewall

Installed directly on a computer or server.

Examples:

Windows Defender Firewall
Linux host firewall

It can protect an individual device even when that device moves between different networks.

Network-Based Firewall

Usually placed at a network boundary and protects multiple systems.

Internet
    │
    ▼
Network Firewall
    │
 ┌──┼───────────┐
 ▼  ▼           ▼
PC  Server    Printer

---

# 💼 Firewall Example

Suppose an organization has a web server that should be accessible from the Internet only through HTTPS.

Internet
   │
   ▼
Firewall
   │
   ├── TCP 443 ──► Allow
   │
   ├── Unnecessary Ports ──► Block
   │
   ▼
Web Server

The firewall reduces the number of services that are directly exposed to untrusted networks.

---

# 🔧 Firewall Security Best Practices

Organizations should:

Allow only necessary traffic.
Block unnecessary services and ports.
Use clear and specific firewall rules.
Review rules regularly.
Remove outdated or unused rules.
Keep firewall software and firmware updated.
Enable appropriate logging and monitoring.
Restrict administrative access.
Use strong administrator authentication and MFA where supported.
Separate network zones when appropriate.
Test firewall configurations.
Follow the principle of least privilege.

---

# ⚠️ Limitations of Firewalls

A firewall is an important security control, but it cannot provide complete security by itself.

A firewall may not prevent:

Phishing attacks
Social engineering
Malware executed by an authorized user
Attacks that use permitted traffic
Compromised credentials
Insider threats
Vulnerabilities in allowed applications

Therefore, firewalls should be combined with other controls such as:

Endpoint protection
MFA
IDS/IPS
Network monitoring
Secure configuration
Patch management
User awareness training
Backups

---

🔐 Firewall and the CIA Triad

| CIA Objective       | Firewall Contribution                                                      |
| ------------------- | -------------------------------------------------------------------------- |
| **Confidentiality** | Can restrict unauthorized network access.                                  |
| **Integrity**       | Can limit unauthorized connections that could lead to modification.        |
| **Availability**    | Can block certain unwanted or malicious traffic that may disrupt services. |

---

# 🚨 Basic Firewall Troubleshooting

When legitimate traffic is blocked:

Check the source and destination addresses.
Verify the required port and protocol.
Review firewall rules.
Check rule order and precedence.
Review firewall logs.
Confirm that the service is actually running.
Test connectivity from the appropriate network.
Make the smallest required rule change.
Document the change.

Avoid simply disabling the firewall to solve a connectivity problem.

---

# 💼 Real-World Applications

Firewalls are commonly used in:

Home networks
Corporate networks
Data centers
Cloud environments
Servers
Wireless networks
Government systems
Educational institutions
Internet gateways

---

# 🛠️ Skills You'll Gain

After completing this section, you'll be able to:

Define a firewall.
Explain how firewalls control network traffic.
Understand firewall rules and filtering.
Differentiate between stateful and stateless firewalls.
Differentiate between host-based and network-based firewalls.
Identify basic firewall security practices.
Understand firewall limitations.
Perform basic firewall troubleshooting.

---

# 📌 Key Takeaways

A firewall monitors and controls network traffic according to security rules.
Firewalls can allow, block, reject, and log traffic.
Rules can use IP addresses, ports, protocols, connection state, and application information.
Common types include packet-filtering, stateful, proxy, and next-generation firewalls.
Firewalls can be host-based or network-based.
A secure configuration should follow least privilege and allow only required traffic.
Firewall rules should be regularly reviewed, updated, tested, and monitored.
A firewall is only one layer of defense and should be combined with other security controls.

---

# 📚 References

- NIST Cybersecurity Framework
- NIST SP 800-41 – Guidelines on Firewalls and Firewall Policy
- CISA – Network Security Guidance
- Microsoft Learn – Windows Defender Firewall
