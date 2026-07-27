# Nslookup
# 📖 Overview

**Nslookup** (Name Server Lookup) is a command-line utility used to query the **Domain Name System (DNS)**.

It helps network administrators verify whether DNS servers are functioning correctly and whether domain names are being resolved into the correct IP addresses.

Nslookup is one of the primary tools used to troubleshoot DNS-related problems such as incorrect records, failed name resolution, and DNS server connectivity issues.

---

# 🎯 Learning Objectives

After completing this topic, you will be able to:

- Understand what Nslookup is.
- Explain how Nslookup works.
- Perform basic DNS queries.
- Troubleshoot DNS resolution issues.
- Interpret Nslookup results.

---

# 📑 Table of Contents

- What is Nslookup?
- How Nslookup Works
- Why Nslookup is Used
- Common Commands
- Troubleshooting Scenarios
- Limitations
- Example
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is Nslookup?

**Nslookup** is a network utility used to query DNS servers.

It allows administrators to determine:

- Whether a domain name resolves correctly.
- Which IP address is associated with a domain.
- Which DNS server provided the answer.
- Whether reverse DNS records exist.

Unlike **Ping**, Nslookup tests **DNS functionality**, not network connectivity.

---

# ⚙️ How Nslookup Works

When a user enters a domain name, Nslookup:

1. Contacts the configured DNS server.
2. Sends a DNS query.
3. Waits for the DNS response.
4. Displays the resolved IP address and DNS server information.

If the DNS server cannot resolve the name, an error is displayed.

---

# 🎯 Why Nslookup is Used

Network administrators use Nslookup to:

- Verify DNS server operation.
- Resolve domain names to IP addresses.
- Perform reverse DNS lookups.
- Verify DNS records.
- Troubleshoot DNS-related connectivity problems.

---

# 💻 Common Commands

## Resolve a Domain Name

```cmd
nslookup google.com
```

---

## Query a Specific DNS Server

```cmd
nslookup google.com 8.8.8.8
```

---

## Reverse DNS Lookup

```cmd
nslookup 8.8.8.8
```

---

## Enter Interactive Mode

```cmd
nslookup
```

Interactive mode allows multiple DNS queries without restarting the command.

---

# 🔍 Common Troubleshooting Scenarios

## Domain Name Does Not Resolve

Symptoms:

- Website cannot be reached by name.
- Website works when using the IP address.

Possible causes:

- DNS server unavailable.
- Incorrect DNS configuration.
- Missing DNS records.

---

## Incorrect IP Address Returned

Possible causes:

- Outdated DNS records.
- Incorrect DNS configuration.
- DNS cache issues.

---

## DNS Server Not Responding

Possible causes:

- DNS server offline.
- Firewall blocking DNS traffic.
- Incorrect DNS server configured.

---

## Reverse Lookup Failure

Possible causes:

- Missing PTR record.
- Reverse DNS zone not configured.

---

# ⚠️ Limitations

Nslookup has several limitations:

- Tests only DNS functionality.
- Does not verify application availability.
- Does not measure latency.
- Does not diagnose routing problems.

For complete network troubleshooting, use Nslookup together with Ping, Tracert, and IPConfig.

---

# 💻 Example

Resolve a domain name:

```cmd
nslookup openai.com
```

Example output:

```text
Server:  dns.company.local
Address: 192.168.1.1

Non-authoritative answer:
Name:    openai.com
Address: 104.18.xxx.xxx
```

Reverse lookup:

```cmd
nslookup 8.8.8.8
```

---

# 📷 Diagram

![Nslookup](https://github.com/varun-kumar-sec/networking-notes/blob/main/Network%20Troubleshooting/Image/nslookup.jpg?raw=true)

---

# 🎤 Interview Questions

### Beginner

- What is Nslookup?
- What is the primary purpose of Nslookup?
- Which service does Nslookup test?
- What information does Nslookup return?

### Intermediate

- Explain how Nslookup works.
- What is the difference between Ping and Nslookup?
- How can Nslookup help diagnose DNS problems?
- What is a reverse DNS lookup?

---

# 📌 Key Takeaways

- Nslookup is a DNS troubleshooting utility.
- It verifies domain name resolution.
- It can perform both forward and reverse DNS lookups.
- It helps identify DNS server and DNS record problems.
- Nslookup complements tools such as IPConfig, Ping, and Tracert during network troubleshooting.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- Microsoft Learn – Nslookup Command
- RFC 1034 – Domain Names: Concepts and Facilities
- RFC 1035 – Domain Names: Implementation and Specification
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
