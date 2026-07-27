# Netsh
# 📖 Overview

**Netsh (Network Shell)** is a Windows command-line utility used to view, configure, and troubleshoot various network settings.

Unlike tools such as **Ping**, **Tracert**, or **IPConfig**, which primarily display network information, Netsh allows administrators to modify network configurations directly from the command line.

It can be used to manage network interfaces, wireless settings, Windows Firewall, TCP/IP configuration, and reset networking components during troubleshooting.

---

# 🎯 Learning Objectives

After completing this topic, you will be able to:

- Understand what Netsh is.
- Explain how Netsh is used in network troubleshooting.
- Perform common Netsh troubleshooting tasks.
- Reset network components using Netsh.
- Understand the advantages and limitations of Netsh.

---

# 📑 Table of Contents

- What is Netsh?
- Why Netsh is Used
- Common Troubleshooting Commands
- Troubleshooting Scenarios
- Limitations
- Example
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is Netsh?

**Netsh** is a Windows command-line scripting utility that allows administrators to configure and manage networking components.

It provides access to many networking features, including:

- TCP/IP configuration
- Network interfaces
- Wireless LAN profiles
- Windows Firewall
- Routing
- IPv4 and IPv6 settings

Because Netsh can change system settings, many commands require **Administrator privileges**.

---

# 🎯 Why Netsh is Used

Network administrators use Netsh to:

- Reset TCP/IP settings.
- Reset the Windows networking stack.
- View wireless network profiles.
- Manage network interfaces.
- Troubleshoot network configuration issues.
- Configure Windows Firewall settings.

---

# 💻 Common Troubleshooting Commands

## Reset TCP/IP Stack

```cmd
netsh int ip reset
```

Restores TCP/IP settings to their default values.

Useful when network configuration becomes corrupted.

---

## Reset Winsock Catalog

```cmd
netsh winsock reset
```

Repairs problems caused by corrupted Winsock entries.

Often used when applications cannot access the network.

A system restart is usually required.

---

## Display Wireless Profiles

```cmd
netsh wlan show profiles
```

Displays all saved Wi-Fi profiles.

---

## Display Wireless Interface Information

```cmd
netsh wlan show interfaces
```

Displays information about the currently connected wireless adapter.

---

## Display IP Configuration Context

```cmd
netsh interface ip show config
```

Displays IP configuration for network interfaces.

---

## Display Windows Firewall Status

```cmd
netsh advfirewall show allprofiles
```

Displays the current firewall configuration for all profiles.

---

# 🔍 Common Troubleshooting Scenarios

## Internet Not Working After Malware Removal

Possible cause:

- Corrupted Winsock catalog.

Solution:

```cmd
netsh winsock reset
```

Restart the computer after running the command.

---

## Corrupted TCP/IP Configuration

Symptoms:

- Incorrect networking behavior.
- Unable to obtain an IP address.
- Connectivity problems.

Solution:

```cmd
netsh int ip reset
```

---

## Wireless Connection Issues

Use:

```cmd
netsh wlan show interfaces
```

Verify:

- Connected SSID
- Signal strength
- Authentication method
- Radio type

---

## Verify Saved Wi-Fi Networks

Use:

```cmd
netsh wlan show profiles
```

Useful when diagnosing wireless profile problems.

---

## Firewall Troubleshooting

Use:

```cmd
netsh advfirewall show allprofiles
```

Verify whether firewall rules may be blocking communication.

---

# ⚠️ Limitations

Netsh has several limitations:

- Some commands require administrator privileges.
- Incorrect commands may change network configuration.
- Available only on Microsoft Windows.
- Many newer management tasks are now performed using PowerShell.

---

# 💻 Example

Reset the TCP/IP stack:

```cmd
netsh int ip reset
```

Reset Winsock:

```cmd
netsh winsock reset
```

Display saved wireless profiles:

```cmd
netsh wlan show profiles
```

---

# 📷 Diagram

![Netsh](https://github.com/varun-kumar-sec/networking-notes/blob/main/Network%20Troubleshooting/Image/Netsh.png?raw=true)

---

# 🎤 Interview Questions

### Beginner

- What is Netsh?
- Why is Netsh used?
- Which command resets the TCP/IP stack?
- Which command displays saved wireless profiles?

### Intermediate

- Explain the difference between `netsh winsock reset` and `netsh int ip reset`.
- When would you use Netsh during troubleshooting?
- Why do many Netsh commands require administrator privileges?
- How can Netsh help diagnose wireless connectivity problems?

---

# 📌 Key Takeaways

- Netsh is a Windows command-line utility for managing network settings.
- It can configure, display, and repair networking components.
- `netsh int ip reset` restores default TCP/IP settings.
- `netsh winsock reset` repairs Winsock-related network issues.
- Netsh is an advanced troubleshooting tool commonly used by Windows administrators.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- Microsoft Learn – Netsh Command
- Microsoft Learn – Windows Networking Documentation
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
