# Share a Folder in Windows
# 📖 Overview

Windows provides built-in file sharing features that allow users to share folders with other computers on the same network. By sharing a folder, authorized users can access files without needing to copy them to each computer.

When a folder is shared, you can control who has access and what they are allowed to do, such as viewing files or making changes.

---

# 🎯 Learning Objectives

After completing this topic, you will be able to:

- Share a folder in Windows.
- Configure basic sharing settings.
- Assign sharing permissions.
- Access a shared folder from another computer.
- Understand basic file sharing security practices.

---

# 📑 Table of Contents

- Requirements
- Steps to Share a Folder
- Configure Share Permissions
- Access the Shared Folder
- Stop Sharing a Folder
- Best Practices
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# ✅ Requirements

Before sharing a folder, ensure that:

- Both computers are connected to the same network.
- Network Discovery is enabled.
- File and Printer Sharing is enabled.
- You have administrator or appropriate user permissions.
- Windows Firewall allows file sharing.

---

# 🛠️ Steps to Share a Folder

## Step 1: Locate the Folder

Open **File Explorer** and browse to the folder you want to share.

---

## Step 2: Open Folder Properties

Right-click the folder and select:

```text
Properties
```

---

## Step 3: Open the Sharing Tab

Select the:

```text
Sharing
```

tab.

Click either:

```text
Share...
```

or

```text
Advanced Sharing...
```

---

## Step 4: Enable Folder Sharing

If using **Advanced Sharing**:

- Check:

```text
Share this folder
```

- Optionally change the **Share Name** if desired.

---

## Step 5: Configure Share Permissions

Click:

```text
Permissions
```

Assign the appropriate permissions for users or groups.

Common permissions include:

- **Read** – View files and folders.
- **Change** – View, create, modify, and delete files.
- **Full Control** – Complete access, including changing permissions.

Choose permissions based on the level of access required.

---

## Step 6: Save the Settings

Click:

```text
Apply
```

then

```text
OK
```

The folder is now shared on the network.

---

# 🔐 Configure Share Permissions

Sharing permissions determine what network users can do with the shared folder.

| Permission | Description |
|------------|-------------|
| **Read** | View and open files |
| **Change** | Read, create, edit, and delete files |
| **Full Control** | Complete control, including changing permissions |

> **Note:** Share permissions work together with **NTFS permissions**. The most restrictive permission is applied to the user.

---

# 🌐 Access the Shared Folder

From another computer on the same network:

1. Open **File Explorer**.
2. In the address bar, enter:

```text
\\ComputerName
```

or

```text
\\IP_Address
```

Example:

```text
\\Office-PC
```

or

```text
\\192.168.1.25
```

3. Press **Enter**.
4. Open the shared folder.
5. If prompted, enter the appropriate user credentials.

---

# ❌ Stop Sharing a Folder

To stop sharing:

1. Right-click the folder.
2. Select **Properties**.
3. Open the **Sharing** tab.
4. Click **Advanced Sharing**.
5. Clear the **Share this folder** checkbox.
6. Click **Apply** and **OK**.

The folder will no longer be accessible over the network.

---

# 🛡️ Best Practices

When sharing folders:

- Share only folders that need to be accessible.
- Grant the minimum permissions required.
- Avoid giving **Full Control** unless necessary.
- Protect shared folders with strong user accounts and passwords.
- Regularly review shared folders and permissions.
- Remove sharing when it is no longer needed.

---

# 📷 Diagram

![share-a-folder-in-windows](https://github.com/varun-kumar-sec/networking-notes/blob/main/File%20Sharing%20and%20Troubleshooting/Image/share-a-folder-in-windows.png?raw=true)

---

# 🎤 Interview Questions

### Beginner

- How do you share a folder in Windows?
- Where is the folder sharing option located?
- What are the three common sharing permission levels?
- How can another computer access a shared folder?

### Intermediate

- Explain the steps involved in sharing a folder.
- What is the difference between **Read** and **Change** permissions?
- Why should you avoid granting **Full Control** unnecessarily?
- How do you stop sharing a folder?

---

# 📌 Key Takeaways

- Windows allows folders to be shared over a local network using built-in sharing features.
- Folder sharing is configured through the **Sharing** tab in the folder's properties.
- Common share permissions include **Read**, **Change**, and **Full Control**.
- Shared folders can be accessed using the computer name or IP address.
- Following the principle of least privilege helps improve the security of shared resources.

---

# 📚 References

- Microsoft Learn – File and Folder Sharing
- Microsoft Windows Documentation
- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
