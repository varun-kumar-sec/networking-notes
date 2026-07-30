# Check File or Folder Permissions
# 📖 Overview

Windows uses **permissions** to control who can access files and folders and what actions they are allowed to perform. Permissions help protect data by ensuring that only authorized users can view, modify, or delete files.

Before troubleshooting file access issues, it is important to verify the permissions assigned to a file or folder. Incorrect permissions are one of the most common reasons users receive **"Access Denied"** or **"You don't have permission to access this folder"** errors.

---

# 🎯 Learning Objectives

After completing this topic, you will be able to:

- Understand file and folder permissions.
- Check permissions for a file or folder.
- Identify the users and groups that have access.
- Understand common permission levels.
- Recognize permission-related access issues.

---

# 📑 Table of Contents

- What are File Permissions?
- Common Permission Levels
- Steps to Check Permissions
- Understanding the Permission List
- Common Permission Problems
- Best Practices
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🔐 What are File Permissions?

File and folder permissions determine:

- Who can access a file or folder.
- What actions users are allowed to perform.
- Which users are prevented from accessing the resource.

Permissions help secure sensitive information and prevent accidental or unauthorized changes.

---

# 📋 Common Permission Levels

Windows commonly uses the following permission levels:

| Permission | Description |
|------------|-------------|
| **Full Control** | View, modify, delete files, change permissions, and take ownership. |
| **Modify** | Read, write, edit, and delete files. |
| **Read & Execute** | Open and run files or applications. |
| **Read** | View file contents and folder information. |
| **Write** | Create new files and modify existing files without full control. |

---

# 🛠️ Steps to Check File or Folder Permissions

## Step 1: Locate the File or Folder

Open **File Explorer** and browse to the desired file or folder.

---

## Step 2: Open Properties

Right-click the file or folder and select:

```text
Properties
```

---

## Step 3: Open the Security Tab

Select the:

```text
Security
```

tab.

This tab displays the users and groups that have permissions for the selected file or folder.

---

## Step 4: Select a User or Group

Click a user or group name from the list.

Examples:

- Administrators
- Users
- SYSTEM
- Your User Account

---

## Step 5: View Permissions

The permissions assigned to the selected user or group are displayed below.

Example:

```text
✓ Full Control
✓ Modify
✓ Read & Execute
✓ Read
✓ Write
```

Checked boxes indicate the permissions that have been granted.

---

# 👥 Understanding the Permission List

The **Group or User Names** section displays accounts that have access to the resource.

Examples include:

- **Administrators** – Users with administrative privileges.
- **SYSTEM** – The Windows operating system.
- **Users** – Standard user accounts.
- **Authenticated Users** – Users who have successfully logged in.

Each entry may have different permission levels depending on security requirements.

---

# ⚠️ Common Permission Problems

## Access Denied

Occurs when the current user does not have the required permissions.

---

## Missing User Account

The required user or group has not been granted access.

---

## Read-Only Access

The user can view files but cannot modify or delete them.

---

## Incorrect Permission Configuration

Permissions may have been changed accidentally or inherited incorrectly from a parent folder.

---

# 🛡️ Best Practices

When managing permissions:

- Grant only the permissions users need.
- Avoid giving **Full Control** unless necessary.
- Regularly review permissions on shared folders.
- Remove unnecessary user accounts.
- Verify permissions before troubleshooting ownership issues.

---

# 📷 Diagram

![check-file-folder-permission](https://github.com/varun-kumar-sec/networking-notes/blob/main/File%20Sharing%20and%20Troubleshooting/Image/Check%20file%20folder%20permission.png?raw=true)

---

# 🎤 Interview Questions

### Beginner

- What are file permissions?
- Which tab is used to view permissions?
- What does the **Read** permission allow?
- Which permission provides complete access?

### Intermediate

- Explain the steps to check file or folder permissions.
- What is the difference between **Modify** and **Full Control**?
- Why might a user receive an **Access Denied** error?
- Why is the principle of least privilege important when assigning permissions?

---

# 📌 Key Takeaways

- File and folder permissions control who can access and modify resources.
- Permissions are viewed through the **Security** tab in the file or folder properties.
- Common permission levels include **Read**, **Write**, **Modify**, and **Full Control**.
- Incorrect permissions are a common cause of file access problems.
- Reviewing permissions is an important step in troubleshooting file sharing issues.

---

# 📚 References

- Microsoft Learn – NTFS Permissions Documentation
- Microsoft Windows Documentation
- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
