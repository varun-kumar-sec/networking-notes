# ⚙️ IP Address Configuration

An IP address alone is not enough for a device to communicate over a network. A device also requires additional network settings, such as the subnet mask, default gateway, and DNS server.

The process of assigning these network settings to a device is called **IP Address Configuration**.

There are two primary methods of configuring an IP address:

- **Manual IP Configuration (Static IP)**
- **Automatic IP Configuration (DHCP)**

This directory explains both methods, their advantages, limitations, and the scenarios in which each is commonly used.

---

## 📂 Directory Structure

```text
07-ip-address-configuration/
│
├── README.md
├── Manual IP Configuration/
│   └── README.md
│
└── Automatic IP Configuration (DHCP)/
    └── README.md
```

---

## 📚 Topics Covered

### 🔹 Manual IP Configuration

Learn about:

- Static IP Address
- Manual network configuration
- Required network settings
- Advantages
- Limitations
- Real-world applications

---

### 🔹 Automatic IP Configuration (DHCP)

Learn about:

- Dynamic IP Address
- DHCP-based configuration
- Automatically assigned network settings
- Advantages
- Limitations
- Real-world applications

---

## ⚖️ Static IP vs Dynamic IP

| Feature | Static IP | Dynamic IP |
|---------|-----------|------------|
| Assignment | Manual | Automatic (DHCP) |
| IP Address | Fixed | Can change |
| Administration | Manual | Automatic |
| Duplicate IP Risk | Higher if misconfigured | Very low |
| Best For | Servers, Printers, Routers | Client Devices |
| Management | Time-consuming | Easy |
| Scalability | Lower | Higher |

---

## 🎯 Learning Objectives

After completing this directory, you will be able to:

- Understand the purpose of IP address configuration.
- Differentiate between static and dynamic IP addressing.
- Identify the information required for IP configuration.
- Explain how DHCP automates IP assignment.
- Choose the appropriate configuration method for different network environments.

---

## 📖 Prerequisites

Before studying this directory, you should understand:

- What is an IP Address?
- IPv4
- Public vs Private IP Address

---

## 🎓 Recommended Study Order

1. Manual IP Configuration
2. Automatic IP Configuration (DHCP)

---

## 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- RFC 2131 – Dynamic Host Configuration Protocol
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
