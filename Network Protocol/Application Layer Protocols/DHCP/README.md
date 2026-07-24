# Dynamic Host Configuration Protocol (DHCP)
# 📖 Overview

The **Dynamic Host Configuration Protocol (DHCP)** is a network management protocol that automatically assigns **IP addresses** and other network configuration information to devices connected to a network.

Without DHCP, network administrators would have to manually configure the IP address, subnet mask, default gateway, and DNS server for every device, which becomes difficult to manage in large networks.

DHCP simplifies network administration by dynamically assigning these settings whenever a device joins the network.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What is DHCP?
- Why DHCP is used
- How DHCP works
- DHCP message exchange (DORA Process)
- Advantages and limitations
- Real-world applications

---

# 📑 Table of Contents

- What is DHCP?
- Why is DHCP Needed?
- How DHCP Works
- DORA Process
- DHCP Lease
- Advantages
- Limitations
- Real-World Applications
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is DHCP?

**DHCP (Dynamic Host Configuration Protocol)** is a protocol that automatically provides network configuration to devices.

Instead of manually configuring every device, a DHCP server assigns:

- IP Address
- Subnet Mask
- Default Gateway
- DNS Server Address
- Lease Time

This allows devices to communicate on the network without manual configuration.

---

# ❓ Why is DHCP Needed?

DHCP is important because it:

- Eliminates manual IP configuration.
- Reduces configuration errors.
- Prevents duplicate IP addresses.
- Simplifies network administration.
- Supports large enterprise networks.

---

# ⚙️ How DHCP Works

When a device connects to a network, it usually does not have an IP address.

It sends a request to the DHCP server, which responds by assigning the necessary network configuration.

This communication follows a four-step process known as **DORA**.

---

# 🔄 DORA Process

The DHCP communication process consists of four messages:

## 1. Discover

The client broadcasts a **DHCP Discover** message to locate available DHCP servers.

↓

## 2. Offer

A DHCP server responds with a **DHCP Offer**, proposing an available IP address and network settings.

↓

## 3. Request

The client sends a **DHCP Request**, indicating that it wants to use the offered IP address.

↓

## 4. Acknowledge

The server sends a **DHCP Acknowledgment (ACK)** confirming the lease and providing the final network configuration.

---

# ⏳ DHCP Lease

A DHCP-assigned IP address is not permanent.

Instead, it is leased for a specific period called the **Lease Time**.

Before the lease expires, the client attempts to renew it automatically.

If the client disconnects permanently, the DHCP server can assign the IP address to another device.

---

# 📡 Default Ports

| Device | Protocol | Port |
|---------|----------|-----:|
| DHCP Server | UDP | 67 |
| DHCP Client | UDP | 68 |

---

# ✅ Advantages

- Automatic IP address assignment.
- Reduces manual configuration.
- Prevents IP conflicts.
- Simplifies network management.
- Supports dynamic environments.
- Efficient use of available IP addresses.

---

# ❌ Limitations

- Requires a DHCP server.
- If the DHCP server becomes unavailable, new devices may not obtain an IP address.
- Less suitable when devices require permanent IP addresses (such as servers).

---

# 🌍 Real-World Applications

DHCP is widely used in:

- Home Wi-Fi networks
- Corporate LANs
- Universities
- Hotels
- Airports
- Public Wi-Fi hotspots
- Enterprise networks

---

# 📷 Diagram

Save the diagram as:

```text
images/dhcp-dora-process.png
```

Recommended diagram:

```text
Client                     DHCP Server
   |                             |
   |---- DHCP Discover --------->|
   |<----- DHCP Offer -----------|
   |---- DHCP Request ---------->|
   |<------ DHCP ACK ------------|
```

Suggested sources:

- https://commons.wikimedia.org/wiki/Category:Dynamic_Host_Configuration_Protocol
- https://en.wikipedia.org/wiki/Dynamic_Host_Configuration_Protocol

---

# 🎤 Interview Questions

### Beginner

- What is DHCP?
- Which ports does DHCP use?
- What does DHCP automatically assign?
- What does DORA stand for?

### Intermediate

- Explain the DORA process.
- What is a DHCP lease?
- Why is DHCP preferred over manual IP configuration?
- What happens if the DHCP server is unavailable?

---

# 📌 Key Takeaways

- DHCP stands for **Dynamic Host Configuration Protocol**.
- It automatically assigns IP addresses and other network settings.
- DHCP uses **UDP Port 67** (Server) and **UDP Port 68** (Client).
- The four-step DHCP communication process is **DORA**:
  - Discover
  - Offer
  - Request
  - Acknowledge
- DHCP simplifies network administration and prevents IP address conflicts.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- RFC 2131 – Dynamic Host Configuration Protocol
- RFC 2132 – DHCP Options and BOOTP Vendor Extensions
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
