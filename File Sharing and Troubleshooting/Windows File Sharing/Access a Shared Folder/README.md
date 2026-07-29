# Access a Shared Folder
# 📖 Overview

After a folder has been shared on a computer, other users on the same network can access it to view, copy, or modify files based on the permissions assigned by the owner.

Windows allows users to access shared folders using either the **computer name** or the **IP address** of the host computer. If the appropriate permissions have been granted, users can easily access shared resources through **File Explorer**.

---

# 🎯 Learning Objectives

After completing this topic, you will be able to:

- Access a shared folder using the computer name.
- Access a shared folder using an IP address.
- Connect to a shared folder using File Explorer.
- Understand when login credentials are required.
- Troubleshoot common access problems.

---

# 📑 Table of Contents

- Requirements
- Access Using the Computer Name
- Access Using the IP Address
- Using Network Discovery
- Access Credentials
- Common Access Problems
- Best Practices
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# ✅ Requirements

Before accessing a shared folder, ensure that:

- Both computers are connected to the same network.
- The folder has been shared.
- Network Discovery is enabled.
- File and Printer Sharing is enabled.
- You have permission to access the shared folder.
- The host computer is powered on and connected to the network.

---

# 🛠️ Access Using the Computer Name

Windows allows shared folders to be accessed using the host computer's name.

## Steps

1. Open **File Explorer**.
2. Click the address bar.
3. Enter:

```text
\\ComputerName
```

Example:

```text
\\Office-PC
```

4. Press **Enter**.
5. Open the desired shared folder.

If required, enter the username and password of the host computer.

---

# 🌐 Access Using the IP Address

If the computer name cannot be resolved, you can use the host computer's IP address.

## Steps

Open **File Explorer** and enter:

```text
\\IP_Address
```

Example:

```text
\\192.168.1.20
```

Press **Enter** to display the available shared folders.

---

# 🖥️ Using Network Discovery

If **Network Discovery** is enabled:

1. Open **File Explorer**.
2. Select:

```text
Network
```

from the navigation pane.

3. Windows displays available computers on the local network.
4. Double-click the desired computer.
5. Open the shared folder.

---

# 🔐 Access Credentials

Some shared folders require user authentication.

When prompted, enter:

- Username
- Password

of an account that has permission to access the shared folder.

Windows may offer the option to remember these credentials for future connections.

---

# ⚠️ Common Access Problems

## Shared Folder Not Found

Possible causes:

- Incorrect computer name.
- Incorrect IP address.
- Folder is no longer shared.

---

## Access Denied

Possible causes:

- Insufficient permissions.
- Incorrect username or password.
- NTFS or Share permissions are restricting access.

---

## Computer Not Visible on the Network

Possible causes:

- Network Discovery is disabled.
- Computer is offline.
- Firewall is blocking network discovery.

---

## Unable to Connect

Possible causes:

- Network connectivity problems.
- Incorrect IP configuration.
- File and Printer Sharing is disabled.

---

# 🛡️ Best Practices

When accessing shared folders:

- Access only folders you are authorized to use.
- Avoid modifying files unless necessary.
- Disconnect from unused shared folders.
- Use secure passwords for shared resources.
- Verify permissions before sharing sensitive information.

---

# 📷 Diagram

Save the diagram as:

```text
images/access-shared-folder.png
```

Recommended diagram:

```text
Computer A
(Shared Folder)
      │
      │  Shared over LAN
      ▼
=============================
        Local Network
=============================
      ▲
      │
Computer B

Open File Explorer

\\Office-PC

or

\\192.168.1.20

        ▼

Access Shared Folder
```

Suggested sources:

- https://learn.microsoft.com/windows/
- https://support.microsoft.com/

---

# 🎤 Interview Questions

### Beginner

- How can you access a shared folder in Windows?
- What are the two common methods of locating a shared folder?
- What is Network Discovery?
- When are login credentials required?

### Intermediate

- Explain the steps for accessing a shared folder using the computer name.
- Why might you use an IP address instead of a computer name?
- What causes an "Access Denied" error when opening a shared folder?
- How would you troubleshoot a shared folder that cannot be found?

---

# 📌 Key Takeaways

- Shared folders can be accessed using either the **computer name** or the **IP address** of the host computer.
- **Network Discovery** allows Windows to automatically display available computers on the local network.
- Access permissions determine whether users can view or modify shared files.
- Authentication may be required before accessing protected shared folders.
- Verifying network connectivity and sharing settings helps resolve most access issues.

---

# 📚 References

- Microsoft Learn – File Sharing Documentation
- Microsoft Windows Documentation
- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
