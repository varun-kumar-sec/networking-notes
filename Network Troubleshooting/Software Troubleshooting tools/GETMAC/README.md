# Getmac
# 📖 Overview

**Getmac** is a Windows command-line utility used to display the **Media Access Control (MAC) addresses** of network adapters.

During troubleshooting, Getmac helps administrators identify the physical address of network interfaces, verify adapter information, and troubleshoot issues involving DHCP reservations, MAC filtering, and network inventory.

Unlike **IPConfig**, which focuses on IP configuration, Getmac provides information about the **hardware (Layer 2)** addresses assigned to network adapters.

---

# 🎯 Learning Objectives

After completing this topic, you will be able to:

- Understand what Getmac is.
- Explain the purpose of a MAC address.
- Use Getmac to identify network adapters.
- Apply Getmac during network troubleshooting.
- Understand the limitations of the command.

---

# 📑 Table of Contents

- What is Getmac?
- Why Getmac is Used
- Basic Syntax
- Common Troubleshooting Scenarios
- Limitations
- Example
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is Getmac?

**Getmac** is a Windows command-line utility that displays the **MAC addresses** of installed network adapters.

A MAC address is a unique hardware identifier assigned to a network interface by the manufacturer.

Network administrators use Getmac to quickly determine the physical address of a computer's network adapters.

---

# 🎯 Why Getmac is Used

Getmac is useful for:

- Identifying network adapters.
- Verifying MAC addresses.
- Troubleshooting DHCP reservations.
- Checking MAC filtering configurations.
- Identifying the correct network interface.
- Maintaining hardware inventories.

---

# 💻 Basic Syntax

Display MAC addresses:

```cmd
getmac
```

Display detailed information:

```cmd
getmac /v
```

Display output in table format:

```cmd
getmac /fo table
```

Common output formats include:

- Table
- List
- CSV

---

# 🔍 Common Troubleshooting Scenarios

## Verify the Correct Network Adapter

If multiple network adapters exist (Ethernet, Wi-Fi, VPN), Getmac helps identify the correct one.

---

## DHCP Reservation Verification

Many DHCP servers assign reserved IP addresses based on the client's MAC address.

Use Getmac to verify that the correct MAC address has been configured.

---

## MAC Address Filtering

Some wireless networks allow only approved MAC addresses.

Getmac helps verify whether the client's MAC address matches the allowed list.

---

## Hardware Inventory

Administrators often use Getmac to document:

- Desktop computers
- Laptops
- Servers
- Virtual machines

---

# ⚠️ Limitations

Getmac has several limitations:

- Displays MAC addresses only.
- Does not test network connectivity.
- Does not display routing information.
- Does not diagnose network failures.
- Does not replace IPConfig or Ping.

---

# 💻 Example

Display installed MAC addresses:

```cmd
getmac
```

Verbose output:

```cmd
getmac /v
```

Example output:

```text
Physical Address    Transport Name

00-15-5D-3A-2B-10   Media Connected
D4-3D-7E-4C-91-55   Media Disconnected
```

---

# 📷 Diagram

Save the diagram as:

```text
images/getmac-troubleshooting.png
```

Recommended diagram:

```text
Computer

Network Adapter

MAC Address

00-15-5D-3A-2B-10

Getmac

        │

Displays Physical Address
```

Suggested sources:

- https://learn.microsoft.com/windows-server/administration/windows-commands/getmac
- https://en.wikipedia.org/wiki/MAC_address

---

# 🎤 Interview Questions

### Beginner

- What is Getmac?
- What information does Getmac display?
- What is a MAC address?
- Why is a MAC address important?

### Intermediate

- How can Getmac help troubleshoot DHCP reservations?
- Why is Getmac useful in MAC filtering environments?
- What is the difference between IPConfig and Getmac?
- Can Getmac diagnose connectivity problems? Why or why not?

---

# 📌 Key Takeaways

- Getmac displays the MAC addresses of network adapters.
- It helps identify physical network interfaces.
- It is useful for DHCP reservations, MAC filtering, and hardware inventory.
- Getmac operates at the Data Link Layer (Layer 2).
- It complements tools like IPConfig and Ping but does not test connectivity.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- Microsoft Learn – Getmac Command
- IEEE 802 Standards
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
