# Manual IP Configuration (Static IP Address)
# 📖 Overview

**Manual IP Configuration**, also known as **Static IP Configuration**, is the process of manually assigning network settings to a device instead of obtaining them automatically.

In this method, the network administrator or user manually enters the required networking information such as the IP address, subnet mask, default gateway, and DNS server.

Static IP addresses are commonly used for servers, printers, routers, switches, and other devices that require a fixed network identity.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What is Manual IP Configuration?
- What is a Static IP Address?
- Information required for manual configuration
- How manual configuration works
- Advantages and limitations
- Common use cases

---

# 📑 Table of Contents

- What is Manual IP Configuration?
- Required Network Information
- How Manual Configuration Works
- Advantages
- Limitations
- Real-World Applications
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is Manual IP Configuration?

Manual IP Configuration is the process of **manually assigning network settings** to a device.

Instead of requesting an IP address from a DHCP server, the user enters all networking parameters manually.

This results in a **Static IP Address**, meaning the device keeps the same IP address until it is changed manually.

---

# 📝 Required Network Information

To manually configure an IP address, the following information is typically required:

### 1. IP Address

Uniquely identifies the device.

Example:

```text
192.168.1.10
```

---

### 2. Subnet Mask

Defines which part of the IP address represents the network and which part represents the host.

Example:

```text
255.255.255.0
```

---

### 3. Default Gateway

Specifies the router used to communicate with other networks.

Example:

```text
192.168.1.1
```

---

### 4. DNS Server

Used to translate domain names into IP addresses.

Example:

```text
8.8.8.8
```

---

# ⚙️ How Manual Configuration Works

The configuration process generally follows these steps:

1. Open the network settings of the device.
2. Select manual (static) IP configuration.
3. Enter the IP address.
4. Enter the subnet mask.
5. Enter the default gateway.
6. Enter the DNS server.
7. Save the configuration.

The device will continue using these settings until they are changed manually.

---

# ✅ Advantages

- IP address remains fixed.
- Ideal for servers and network devices.
- Easy to locate important devices.
- No dependency on a DHCP server.
- Useful for services that require a permanent IP address.

---

# ❌ Limitations

- Time-consuming to configure.
- Requires manual management.
- Higher chance of configuration errors.
- Duplicate IP addresses can occur if not managed properly.
- Less practical for large networks.

---

# 🌍 Real-World Applications

Static IP addresses are commonly used for:

- Web servers
- Database servers
- Mail servers
- Network printers
- Routers
- Switches
- Firewalls
- CCTV systems

---

# 📷 Diagram

Save the diagram as:

```text
images/manual-ip-configuration.png
```

Recommended diagram:

```text
Computer

IP Address:
192.168.1.10

Subnet Mask:
255.255.255.0

Gateway:
192.168.1.1

DNS:
8.8.8.8

↓

Configured Manually
```

Suggested sources:

- https://commons.wikimedia.org/wiki/Category:Internet_Protocol
- https://en.wikipedia.org/wiki/IP_address

---

# 🎤 Interview Questions

### Beginner

- What is Manual IP Configuration?
- What is a Static IP Address?
- What information is required for manual configuration?
- Why is a default gateway required?

### Intermediate

- When should a static IP address be used?
- What problems can occur with manual configuration?
- Why are servers commonly assigned static IP addresses?
- What happens if two devices are configured with the same static IP address?

---

# 📌 Key Takeaways

- Manual IP Configuration assigns network settings manually.
- A manually assigned IP address is called a **Static IP Address**.
- Configuration requires an IP address, subnet mask, default gateway, and DNS server.
- Static IP addresses remain unchanged until manually modified.
- Manual configuration is commonly used for servers, printers, routers, and other critical network devices.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
