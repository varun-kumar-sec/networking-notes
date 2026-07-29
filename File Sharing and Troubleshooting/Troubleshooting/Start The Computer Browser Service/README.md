# Start the Computer Browser Service in Windows

> **Module:** File Sharing and Troubleshooting  
> **Section:** Troubleshooting  
> **Difficulty:** Beginner  
> **Prerequisites:** Troubleshooting File Sharing Issues  
> **Estimated Reading Time:** 7–9 Minutes

---

# 📖 Overview

The **Computer Browser** service was a Windows networking service that maintained a list of computers and shared resources available on a local network. It helped users browse computers through the **Network** section of File Explorer.

If the service was stopped on older versions of Windows, computers might not appear in the network browser even though they were connected and functioning correctly.

> **Important:** The **Computer Browser** service has been **removed in modern versions of Windows (Windows 10 version 1709 and later, Windows 11, and Windows Server 2019 and later)**. Modern Windows systems use newer technologies such as **Function Discovery** and **SMB** for network discovery. You may still encounter the Computer Browser service on older Windows versions during legacy system support.

---

# 🎯 Learning Objectives

After completing this topic, you will be able to:

- Understand the purpose of the Computer Browser service.
- Determine when the service is applicable.
- Start the Computer Browser service on supported Windows versions.
- Verify whether the service is running.
- Understand modern alternatives used in current Windows versions.

---

# 📑 Table of Contents

- What is the Computer Browser Service?
- When is it Used?
- Steps to Start the Service
- Verify the Service Status
- Modern Windows Alternatives
- Best Practices
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🖥️ What is the Computer Browser Service?

The **Computer Browser** service collected and maintained a list of computers and shared resources on a local network.

It allowed users to:

- View computers under **Network** in File Explorer.
- Discover shared folders.
- Browse network resources without manually entering computer names or IP addresses.

This service primarily worked in Windows workgroup environments.

---

# 📅 When is it Used?

You may encounter the Computer Browser service when:

- Supporting older Windows operating systems.
- Troubleshooting legacy workgroup networks.
- Maintaining older office or laboratory computers.

For modern Windows environments, this service is **not available** and should not be considered a troubleshooting requirement.

---

# 🛠️ Steps to Start the Computer Browser Service

> **Note:** These steps apply only to Windows versions that still include the Computer Browser service.

## Step 1: Open the Services Console

Press:

```text
Windows + R
```

Type:

```text
services.msc
```

Click:

```text
OK
```

---

## Step 2: Locate the Service

Scroll through the list and locate:

```text
Computer Browser
```

---

## Step 3: Open Service Properties

Double-click the service.

The properties window displays:

- Service status
- Startup type
- Dependencies

---

## Step 4: Start the Service

If the service is stopped:

Click:

```text
Start
```

Set the **Startup type** to:

```text
Automatic
```

or

```text
Manual
```

depending on your organization's requirements.

Click:

```text
Apply
```

then

```text
OK
```

---

# ✅ Verify the Service Status

The **Status** column in the Services console should display:

```text
Running
```

You can also verify by checking whether network computers become visible in **File Explorer → Network** on supported systems.

---

# 🔄 Modern Windows Alternatives

Current versions of Windows no longer include the Computer Browser service.

Instead, network discovery relies on:

- **Function Discovery Provider Host**
- **Function Discovery Resource Publication**
- **Server** service
- **Workstation** service
- **SMB (Server Message Block)** protocol
- **Network Discovery** feature

When troubleshooting file sharing on Windows 10, Windows 11, or Windows Server 2019 and later, these components are more relevant than the Computer Browser service.

---

# 🛡️ Best Practices

When troubleshooting network discovery:

- Verify **Network Discovery** is enabled.
- Ensure **File and Printer Sharing** is enabled.
- Confirm required Windows services are running.
- Keep Windows updated.
- Use modern network discovery methods instead of relying on legacy services.
- Only enable legacy services when supporting older operating systems.

---

# 📷 Diagram

Save the diagram as:

```text
images/computer-browser-service.png
```

Recommended diagram:

```text
Windows + R
      │
      ▼
services.msc
      │
      ▼
Services Console
      │
      ▼
Computer Browser
      │
      ▼
Start Service
      │
      ▼
Status = Running
      │
      ▼
Legacy Network Discovery
```

Suggested sources:

- https://learn.microsoft.com/windows/
- https://support.microsoft.com/

---

# 🎤 Interview Questions

### Beginner

- What was the purpose of the Computer Browser service?
- On which types of Windows systems is the Computer Browser service typically found?
- How do you open the Services console?
- Is the Computer Browser service available in modern Windows versions?

### Intermediate

- Explain the steps to start the Computer Browser service.
- Why was the Computer Browser service removed from newer Windows versions?
- Which services have replaced the Computer Browser service in modern Windows?
- Why should you avoid relying on the Computer Browser service when troubleshooting Windows 11?

---

# 📌 Key Takeaways

- The **Computer Browser** service maintained a list of computers and shared resources on older Windows networks.
- It is primarily relevant when supporting legacy Windows systems.
- The service can be managed through the **Services** console (`services.msc`) on supported versions.
- Modern Windows versions use **Function Discovery**, **SMB**, and **Network Discovery** instead of the Computer Browser service.
- When troubleshooting current Windows systems, focus on modern networking services rather than legacy components.

---

# 📚 References

- Microsoft Learn – Windows Networking Documentation
- Microsoft Windows Documentation
- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
