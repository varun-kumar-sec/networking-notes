# ipconfig Command
# 📖 Overview

The **ipconfig** command is a built-in Windows command-line utility used to display and manage the IP configuration of a computer.

It helps users and network administrators verify network settings, troubleshoot connectivity issues, and manage DHCP-assigned IP addresses.

The command is commonly executed from **Command Prompt (CMD)** or **Windows Terminal**.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What is the ipconfig command?
- Why ipconfig is used
- Basic ipconfig syntax
- Common ipconfig options
- Real-world applications

---

# 📑 Table of Contents

- What is ipconfig?
- Why Use ipconfig?
- Basic Syntax
- Common Commands
- Real-World Applications
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 💻 What is ipconfig?

**ipconfig** is a Windows networking utility that displays the current IP configuration of network adapters.

It can also be used to:

- Renew DHCP leases
- Release DHCP leases
- Display detailed network information
- Flush the DNS cache

---

# ❓ Why Use ipconfig?

The ipconfig command helps users:

- Verify IP configuration
- Check the assigned IP address
- View the subnet mask
- View the default gateway
- View DNS server information
- Troubleshoot network problems

---

# ⚙️ Basic Syntax

```cmd
ipconfig
```

Displays basic IP configuration.

---

# 📋 Common ipconfig Commands

## Display Basic Configuration

```cmd
ipconfig
```

Displays:

- IPv4 Address
- Subnet Mask
- Default Gateway

---

## Display Detailed Configuration

```cmd
ipconfig /all
```

Displays additional information such as:

- Host Name
- Physical (MAC) Address
- DHCP Enabled
- DHCP Server
- DNS Servers
- Lease Information

---

## Release DHCP Address

```cmd
ipconfig /release
```

Releases the current DHCP-assigned IP address.

---

## Renew DHCP Address

```cmd
ipconfig /renew
```

Requests a new IP configuration from the DHCP server.

---

## Flush DNS Cache

```cmd
ipconfig /flushdns
```

Clears the locally cached DNS records.

Useful when:

- DNS entries are outdated.
- Websites fail to resolve correctly.
- DNS troubleshooting is required.

---

# 🌍 Real-World Applications

The ipconfig command is commonly used to:

- Verify IP configuration
- Check DHCP operation
- Troubleshoot network connectivity
- Diagnose incorrect IP settings
- Refresh a DHCP lease
- Resolve DNS-related issues

---

# 📷 Diagram

![Ipconfig](https://github.com/varun-kumar-sec/networking-notes/blob/main/IP%20Addressing/Image/ipconfig.png?raw=true)

---

# 🎤 Interview Questions

### Beginner

- What is the ipconfig command?
- Which operating system provides ipconfig?
- Which command displays detailed network information?
- Which command requests a new DHCP address?

### Intermediate

- What is the difference between `ipconfig` and `ipconfig /all`?
- When would you use `ipconfig /release`?
- Why is `ipconfig /renew` useful?
- What does `ipconfig /flushdns` do?

---

# 📌 Key Takeaways

- **ipconfig** is a Windows command-line networking utility.
- It displays the current IP configuration of network adapters.
- `ipconfig /all` shows detailed network information.
- `ipconfig /release` releases the current DHCP lease.
- `ipconfig /renew` requests a new DHCP lease.
- `ipconfig /flushdns` clears the local DNS cache.

---

# 📚 References

- Microsoft Learn – Windows Commands
- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- Microsoft Windows Documentation
