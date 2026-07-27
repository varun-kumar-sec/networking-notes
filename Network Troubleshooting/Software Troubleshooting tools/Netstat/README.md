# Netstat
# 📖 Overview

**Netstat** (Network Statistics) is a command-line utility used to display active network connections, listening ports, routing tables, and protocol statistics.

It helps network administrators understand how a computer is communicating with other devices and identify issues such as unexpected connections, services that are not listening, or applications using network ports.

Netstat is an essential troubleshooting tool for diagnosing both network and application connectivity problems.

---

# 🎯 Learning Objectives

After completing this topic, you will be able to:

- Understand what Netstat is.
- View active network connections.
- Identify listening ports.
- Display routing information.
- Troubleshoot network communication problems using Netstat.

---

# 📑 Table of Contents

- What is Netstat?
- How Netstat Works
- Why Netstat is Used
- Common Commands
- Troubleshooting Scenarios
- Limitations
- Example
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is Netstat?

**Netstat** is a command-line utility that displays information about a computer's network activity.

It can display:

- Active TCP connections
- Listening ports
- UDP endpoints
- Routing table
- Network interface statistics
- Protocol statistics

Unlike Ping or Tracert, Netstat focuses on the **local computer's network communication**.

---

# ⚙️ How Netstat Works

Netstat reads information from the operating system's networking stack and displays details about:

- Established TCP connections
- Ports currently listening for incoming connections
- Protocol statistics
- Routing information

This helps administrators determine how applications are communicating over the network.

---

# 🎯 Why Netstat is Used

Network administrators use Netstat to:

- View active connections.
- Identify listening ports.
- Troubleshoot application connectivity.
- Detect unauthorized or suspicious connections.
- Verify that network services are running.
- Display routing information.

---

# 💻 Common Commands

## Display Active Connections

```cmd
netstat
```

Displays active TCP connections.

---

## Display All Connections and Listening Ports

```cmd
netstat -a
```

Shows:

- Active connections
- Listening ports
- UDP endpoints

---

## Display Numerical Addresses

```cmd
netstat -n
```

Displays IP addresses and port numbers without resolving hostnames.

---

## Display Executable Associated with Each Connection

```cmd
netstat -b
```

Requires administrator privileges.

Shows which executable created each connection.

---

## Display Process ID (PID)

```cmd
netstat -o
```

Displays the Process ID associated with each connection.

Useful when identifying which application owns a connection.

---

## Display Routing Table

```cmd
netstat -r
```

Displays the system routing table.

---

## Display Ethernet Statistics

```cmd
netstat -e
```

Shows:

- Bytes sent
- Bytes received
- Network errors

---

# 🔍 Common Troubleshooting Scenarios

## Service Not Accessible

Use:

```cmd
netstat -a
```

Verify that the required port is in the **LISTENING** state.

---

## Unexpected Network Connections

Use:

```cmd
netstat -ano
```

Look for unknown or suspicious remote connections.

---

## Identify Application Using a Port

Use:

```cmd
netstat -ano
```

Then match the displayed PID with Task Manager or:

```cmd
tasklist
```

---

## Port Already in Use

If an application cannot start because a port is occupied:

```cmd
netstat -ano
```

Identify which process owns the port.

---

## Routing Verification

Use:

```cmd
netstat -r
```

Confirm that routes have been configured correctly.

---

# ⚠️ Limitations

Netstat has several limitations:

- Displays current network information only.
- Does not test connectivity.
- Does not diagnose DNS issues.
- Cannot identify packet loss.
- May require administrator privileges for some options.

---

# 💻 Example

Display active connections and listening ports:

```cmd
netstat -ano
```

Example output:

```text
Proto  Local Address      Foreign Address    State        PID

TCP    192.168.1.10:80    192.168.1.20:52310 ESTABLISHED  4321
TCP    0.0.0.0:443        0.0.0.0:0          LISTENING    2100
```

---

# 📷 Diagram

![Netstat](https://github.com/varun-kumar-sec/networking-notes/blob/main/Network%20Troubleshooting/Image/netsat.png?raw=true)

---

# 🎤 Interview Questions

### Beginner

- What is Netstat?
- What information does Netstat display?
- What is a listening port?
- Which command displays all active connections?

### Intermediate

- Explain the purpose of `netstat -ano`.
- How can Netstat help identify which application is using a port?
- Why would you use `netstat -r`?
- What is the difference between an ESTABLISHED connection and a LISTENING port?

---

# 📌 Key Takeaways

- Netstat displays active network connections and listening ports.
- It helps identify which applications are communicating over the network.
- It can display routing information, protocol statistics, and process IDs.
- Netstat is useful for diagnosing application connectivity and port-related issues.
- It complements tools such as IPConfig, Ping, Tracert, PathPing, and Nslookup.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- Microsoft Learn – Netstat Command
- RFC 793 – Transmission Control Protocol (TCP)
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
