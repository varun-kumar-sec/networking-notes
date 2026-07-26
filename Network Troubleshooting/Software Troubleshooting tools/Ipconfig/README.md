# IPConfig
# 📖 Overview

**IPConfig** is a Windows command-line utility used to display and manage a computer's TCP/IP network configuration.

From a troubleshooting perspective, IPConfig helps network administrators verify whether a computer has received the correct IP configuration, identify addressing problems, diagnose DHCP issues, and refresh network settings.

It is one of the first commands used when troubleshooting local network connectivity.

---

# 🎯 Learning Objectives

After completing this topic, you will be able to:

- Understand IPConfig as a troubleshooting tool.
- Verify local network configuration.
- Diagnose IP addressing problems.
- Troubleshoot DHCP issues.
- Use common IPConfig troubleshooting options.

---

# 📑 Table of Contents

- What is IPConfig?
- Why IPConfig is Used
- Common Troubleshooting Commands
- Troubleshooting Scenarios
- Best Practices
- Example
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is IPConfig?

**IPConfig** is a Windows command-line utility that displays and manages the TCP/IP configuration of network adapters.

It allows administrators to verify information such as:

- IP Address
- Subnet Mask
- Default Gateway
- DNS Servers
- DHCP Status
- MAC Address (Physical Address)

Unlike Ping or Tracert, IPConfig focuses on the **local computer's network configuration** rather than testing communication across the network.

---

# 🎯 Why IPConfig is Used

Network administrators use IPConfig to:

- Verify IP configuration.
- Confirm DHCP operation.
- Detect incorrect IP settings.
- Check DNS server configuration.
- Refresh IP addresses.
- Diagnose local connectivity issues.

---

# 🛠️ Common Troubleshooting Commands

## Display Basic Configuration

```cmd
ipconfig
```

Displays the IP address, subnet mask, and default gateway.

---

## Display Detailed Information

```cmd
ipconfig /all
```

Displays additional information, including:

- DHCP status
- DNS servers
- Physical (MAC) address
- Lease information
- Adapter description

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

Requests a new IP address from the DHCP server.

---

## Flush DNS Cache

```cmd
ipconfig /flushdns
```

Clears the local DNS resolver cache.

Useful when outdated DNS records cause name resolution problems.

---

## Register DNS

```cmd
ipconfig /registerdns
```

Requests that the computer re-register its DNS records with the configured DNS server.

---

# 🔍 Common Troubleshooting Scenarios

### Incorrect IP Address

Symptoms:

- Unable to reach other devices.
- No Internet access.

Check:

```cmd
ipconfig
```

Verify that the IP address belongs to the correct network.

---

### APIPA Address (169.254.x.x)

An address in the **169.254.x.x** range usually indicates that the computer could not contact a DHCP server.

Possible causes:

- DHCP server unavailable.
- Network cable disconnected.
- Faulty switch port.
- Wireless connection problem.

---

### Incorrect Default Gateway

Symptoms:

- Can access local devices.
- Cannot access remote networks or the Internet.

Use:

```cmd
ipconfig
```

Verify the configured default gateway.

---

### DNS Problems

Symptoms:

- Websites open by IP address but not by name.

Use:

```cmd
ipconfig /flushdns
```

to clear cached DNS records.

---

### DHCP Issues

If a computer receives an incorrect address:

```cmd
ipconfig /release
ipconfig /renew
```

These commands request a new DHCP lease.

---

# ✅ Best Practices

When using IPConfig during troubleshooting:

- Verify the IP address before testing connectivity.
- Confirm the subnet mask and default gateway.
- Check DNS server configuration.
- Use `/all` for complete adapter information.
- Use `/renew` only after confirming DHCP availability.

---

# 💻 Example

Display complete network configuration:

```cmd
ipconfig /all
```

Renew the DHCP lease:

```cmd
ipconfig /release
ipconfig /renew
```

Clear the DNS cache:

```cmd
ipconfig /flushdns
```

---

# 📷 Diagram

Save the diagram as:

```text
images/ipconfig-troubleshooting.png
```

Recommended diagram:

```text
Computer

      │

IPConfig Checks

✔ IP Address
✔ Subnet Mask
✔ Default Gateway
✔ DNS Servers
✔ DHCP Status

      │

Identify Local Configuration Problems
```

Suggested sources:

- https://learn.microsoft.com/windows-server/administration/windows-commands/ipconfig
- https://en.wikipedia.org/wiki/Ipconfig

---

# 🎤 Interview Questions

### Beginner

- What is IPConfig?
- Why is IPConfig used during troubleshooting?
- What does `ipconfig /all` display?
- What is an APIPA address?

### Intermediate

- What is the purpose of `ipconfig /renew`?
- When would you use `ipconfig /flushdns`?
- How can IPConfig help diagnose DHCP problems?
- Why is checking the default gateway important?

---

# 📌 Key Takeaways

- IPConfig is used to view and manage local TCP/IP configuration.
- It helps diagnose IP addressing, DHCP, DNS, and gateway problems.
- `ipconfig /all` displays detailed adapter information.
- `ipconfig /release` and `/renew` are useful for DHCP troubleshooting.
- IPConfig is one of the first tools used to verify local network configuration.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- Microsoft Learn – IPConfig Command
- RFC 2131 – Dynamic Host Configuration Protocol (DHCP)
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
