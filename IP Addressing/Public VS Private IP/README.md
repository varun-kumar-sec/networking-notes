# Public IP vs Private IP Address
# 📖 Overview

IPv4 addresses are divided into two categories:

- **Public IP Addresses**
- **Private IP Addresses**

A **Public IP Address** is globally unique and can communicate over the Internet.

A **Private IP Address** is used within local networks and cannot communicate directly over the Internet.

This distinction helps conserve IPv4 addresses while improving security and network organization.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What is a Public IP Address?
- What is a Private IP Address?
- Differences between Public and Private IPs
- Private IP address ranges
- Why private addresses are used
- The role of NAT

---

# 📑 Table of Contents

- What is a Public IP Address?
- What is a Private IP Address?
- Private IPv4 Address Ranges
- Public vs Private IP Comparison
- Role of NAT
- Real-World Example
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌍 What is a Public IP Address?

A **Public IP Address** is an IP address that is globally unique and accessible over the Internet.

It is assigned by an **Internet Service Provider (ISP)**.

Examples:

```text
8.8.8.8
1.1.1.1
142.250.182.14
```

Public IP addresses are used by:

- Web servers
- Cloud services
- Internet-connected routers
- Public websites

---

# 🏠 What is a Private IP Address?

A **Private IP Address** is used inside a Local Area Network (LAN).

These addresses are **not routable on the public Internet**.

Private IP addresses are commonly assigned by home or office routers.

Examples:

```text
192.168.1.10

10.0.0.25

172.16.5.12
```

---

# 📌 Private IPv4 Address Ranges

RFC 1918 defines three private IPv4 address ranges.

| Range | Address Block |
|--------|---------------|
| Class A | 10.0.0.0 – 10.255.255.255 |
| Class B | 172.16.0.0 – 172.31.255.255 |
| Class C | 192.168.0.0 – 192.168.255.255 |

These addresses are reserved for private networks.

---

# ⚖️ Public vs Private IP

| Feature | Public IP | Private IP |
|---------|-----------|------------|
| Internet Accessible | Yes | No |
| Globally Unique | Yes | No |
| Assigned By | ISP | Router / Network Administrator |
| Used In | Internet | Local Networks |
| Routable | Yes | No |
| Example | 8.8.8.8 | 192.168.1.10 |

---

# 🔄 Role of NAT

Devices with private IP addresses cannot communicate directly over the Internet.

To access the Internet, routers use **Network Address Translation (NAT)**.

NAT temporarily replaces a device's private IP address with the router's public IP address when communicating with external networks.

This allows multiple devices in a private network to share a single public IP address.

---

# 🌍 Real-World Example

Suppose a home network contains:

```text
Laptop
192.168.1.10

Phone
192.168.1.11

Smart TV
192.168.1.12
```

All three devices use private IP addresses.

The home router has one public IP address assigned by the ISP.

When these devices access the Internet, the router performs NAT so that external servers see only the router's public IP address.

---

# 📷 Diagram

![public-vs-private-ip](https://github.com/varun-kumar-sec/networking-notes/blob/main/IP%20Addressing/Image/public-vs-private-ip.jpg?raw=true)

---

# 🎤 Interview Questions

### Beginner

- What is a Public IP Address?
- What is a Private IP Address?
- Name the three private IPv4 address ranges.
- Who assigns a public IP address?

### Intermediate

- Why are private IP addresses used?
- Why can't private IP addresses communicate directly over the Internet?
- What is NAT?
- How does NAT help conserve IPv4 addresses?

---

# 📌 Key Takeaways

- Public IP addresses are globally unique and Internet-routable.
- Private IP addresses are used within local networks.
- RFC 1918 defines three private IPv4 address ranges.
- Private IP addresses require **NAT** to communicate over the Internet.
- Most home and office networks use private IP addressing internally.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- RFC 1918 – Address Allocation for Private Internets
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
