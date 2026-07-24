# 🔍 Verifying IP Configuration

After configuring an IP address, it is important to verify that the device is correctly connected to the network and can communicate with other devices.

Network administrators use various command-line utilities to check IP settings, test connectivity, and diagnose network problems. These tools help identify configuration errors, connectivity issues, and routing problems.

This directory introduces the most commonly used commands for verifying IP configuration and performing basic network troubleshooting.

---

## 📂 Directory Structure

```text
08-verifying-ip-configuration/
│
├── README.md
├── ipconfig/
│   └── README.md
│
├── ping/
│   └── README.md
│
└── traceroute/
    └── README.md
```

---

## 📚 Topics Covered

### 🔹 ipconfig

Learn about:

- Viewing IP configuration
- Displaying detailed network information
- Renewing DHCP leases
- Releasing DHCP leases
- Flushing the DNS cache

---

### 🔹 ping

Learn about:

- Testing network connectivity
- ICMP Echo Request and Echo Reply
- Measuring network latency
- Identifying packet loss
- Troubleshooting communication problems

---

### 🔹 traceroute (tracert)

Learn about:

- Discovering the path to a destination
- Understanding network hops
- Identifying routing problems
- Measuring delay between routers
- Diagnosing network path issues

---

## ⚖️ Command Comparison

| Command | Primary Purpose |
|---------|------------------|
| **ipconfig** | View and manage local IP configuration |
| **ping** | Test connectivity between two devices |
| **traceroute (tracert)** | Display the path packets take through the network |

---

## 🎯 Learning Objectives

After completing this directory, you will be able to:

- Verify the IP configuration of a device.
- Test communication with local and remote hosts.
- Identify basic network connectivity issues.
- Determine the path packets take across a network.
- Use common command-line tools for network verification.

---

## 📖 Prerequisites

Before studying this directory, you should understand:

- IPv4 Addressing
- Public vs Private IP Address
- IP Address Configuration

---

## 🎓 Recommended Study Order

1. ipconfig
2. ping
3. traceroute (tracert)

---

## 💡 When to Use These Commands

| Situation | Recommended Command |
|-----------|---------------------|
| Check your IP address | `ipconfig` |
| Verify Internet or network connectivity | `ping` |
| Find where communication fails | `traceroute` (`tracert` on Windows) |

---

## 📚 References

- Microsoft Learn – Windows Commands
- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- RFC 791 – Internet Protocol (IPv4)
- RFC 792 – Internet Control Message Protocol (ICMP)
