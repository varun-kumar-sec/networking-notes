# Simple Network Management Protocol (SNMP)
# 📖 Overview

The **Simple Network Management Protocol (SNMP)** is an application-layer protocol used to monitor, manage, and configure network devices over an IP network.

SNMP enables network administrators to monitor the health, performance, and status of devices such as routers, switches, servers, printers, firewalls, and wireless access points from a central location.

Instead of manually checking every network device, administrators can use SNMP to collect information and receive alerts whenever a problem occurs.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What is SNMP?
- Why SNMP is used
- How SNMP works
- Components of SNMP
- Default ports
- Advantages and limitations
- Real-world applications

---

# 📑 Table of Contents

- What is SNMP?
- Why is SNMP Needed?
- Components of SNMP
- How SNMP Works
- Default Ports
- Advantages
- Limitations
- Real-World Applications
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is SNMP?

**SNMP (Simple Network Management Protocol)** is a protocol used for monitoring and managing network devices.

It allows administrators to:

- Monitor device performance
- Collect device statistics
- Detect network faults
- Receive alerts
- Configure supported devices remotely

SNMP is commonly used in enterprise networks to simplify network management.

---

# ❓ Why is SNMP Needed?

SNMP is important because it:

- Simplifies network monitoring.
- Detects device failures quickly.
- Provides centralized network management.
- Reduces manual administration.
- Improves network reliability.

---

# 🧩 Components of SNMP

SNMP consists of three main components.

## 1. SNMP Manager

The **Manager** is the central system that monitors and manages network devices.

Examples:

- Network monitoring software
- Management servers

---

## 2. SNMP Agent

An **Agent** is software running on a network device.

Its responsibilities include:

- Collecting device information
- Responding to manager requests
- Sending alerts (Traps)

---

## 3. Managed Device

A managed device is any network device running an SNMP agent.

Examples:

- Router
- Switch
- Firewall
- Server
- Printer
- Wireless Access Point

---

# ⚙️ How SNMP Works

The communication process generally follows these steps:

1. The SNMP Manager sends a request to an SNMP Agent.
2. The Agent retrieves the requested information.
3. The Agent sends the information back to the Manager.
4. If a problem occurs, the Agent automatically sends a **Trap** message to the Manager.

---

# 📡 Default Ports

| Protocol | Port | Purpose |
|----------|-----:|----------|
| UDP | 161 | Communication between Manager and Agent |
| UDP | 162 | SNMP Trap Notifications |

---

# 🔄 SNMP Workflow

```text
             SNMP Manager
                  │
      Request Device Information
                  │
                  ▼
             SNMP Agent
                  │
      Collect Device Statistics
                  │
                  ▼
            Managed Device

If a fault occurs:

Managed Device
      │
      ▼
 SNMP Agent
      │ Trap
      ▼
 SNMP Manager
```

---

# ✅ Advantages

- Centralized network monitoring.
- Simplifies device management.
- Detects faults quickly.
- Supports automation.
- Reduces administrative workload.

---

# ❌ Limitations

- Earlier SNMP versions have limited security.
- Configuration can become complex in large networks.
- Requires SNMP-enabled devices.
- Uses UDP, which does not guarantee delivery.

---

# 🌍 Real-World Applications

SNMP is commonly used for:

- Monitoring routers
- Monitoring switches
- Monitoring servers
- Printer management
- Data center monitoring
- Enterprise network management
- Performance monitoring
- Fault detection

---

# 📷 Diagram

![SNMP](https://github.com/varun-kumar-sec/networking-notes/blob/main/Network%20Protocol/Image/snmp.jpg?raw=true)

---

# 🎤 Interview Questions

### Beginner

- What is SNMP?
- Which ports does SNMP use?
- What is an SNMP Agent?
- What is an SNMP Manager?

### Intermediate

- Explain how SNMP works.
- Differentiate between SNMP Manager and SNMP Agent.
- What is an SNMP Trap?
- Why does SNMP use UDP instead of TCP?

---

# 📌 Key Takeaways

- SNMP stands for **Simple Network Management Protocol**.
- It is used to monitor and manage network devices.
- SNMP uses **UDP Port 161** for communication.
- **UDP Port 162** is used for Trap notifications.
- The three main SNMP components are **Manager**, **Agent**, and **Managed Device**.
- SNMP enables centralized monitoring of enterprise networks.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- RFC 1157 – Simple Network Management Protocol (SNMP)
- RFC 3411 – An Architecture for SNMP Management Frameworks
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
