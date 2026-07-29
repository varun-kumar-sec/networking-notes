# Change the Default Administrator Password
# 📖 Overview

One of the first security tasks after setting up a router is changing the **default administrator password**.

Most routers are shipped with factory-default login credentials, such as **admin/admin** or **admin/password**. These default credentials are widely known and can be easily found in user manuals or on manufacturers' websites.

If the default administrator password is not changed, anyone with access to the network may be able to log in to the router, modify its settings, or compromise the network.

Changing the administrator password helps protect the router from unauthorized access and is considered a basic network security practice.

---

# 🎯 Learning Objectives

After completing this topic, you will be able to:

- Understand why the default administrator password should be changed.
- Change the administrator password on a router.
- Create a strong administrator password.
- Differentiate between the administrator password and the Wi-Fi password.
- Apply security best practices for router administration.

---

# 📑 Table of Contents

- Why Change the Default Password?
- Administrator Password vs Wi-Fi Password
- Steps to Change the Administrator Password
- Creating a Strong Password
- Best Practices
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🔒 Why Change the Default Password?

Default administrator credentials are publicly available and commonly targeted by attackers.

Leaving the default password unchanged can allow unauthorized users to:

- Change router settings.
- Disable network security.
- Change the Wi-Fi password.
- Block Internet access.
- Redirect network traffic.
- Install malicious configurations.

Changing the administrator password significantly improves router security.

---

# 👤 Administrator Password vs Wi-Fi Password

These two passwords serve different purposes.

| Administrator Password | Wi-Fi Password |
|-------------------------|----------------|
| Protects access to the router's management interface | Protects access to the wireless network |
| Used by administrators | Used by wireless users |
| Controls router settings | Allows devices to join the Wi-Fi network |

Changing the Wi-Fi password **does not** change the administrator password, and vice versa.

---

# 🛠️ Steps to Change the Administrator Password

## Step 1: Access the Router

Open a web browser and enter the router's management IP address.

Example:

```text
192.168.0.1
192.168.1.1
```

Log in using the current administrator credentials.

---

## Step 2: Open Administration Settings

Navigate to the router's administration or management section.

Depending on the manufacturer, this may be labeled:

- Administration
- System
- Management
- Device Settings

---

## Step 3: Enter a New Password

Create a new administrator password.

Most routers require:

- Current password
- New password
- Password confirmation

---

## Step 4: Save the Changes

Click:

```text
Save
```

or

```text
Apply
```

The router may require you to log in again using the new password.

---

# 🔑 Creating a Strong Administrator Password

A strong administrator password should:

- Be at least 12 characters long.
- Include uppercase letters.
- Include lowercase letters.
- Include numbers.
- Include special characters.
- Be unique and difficult to guess.

Example:

```text
R0ut3r@Secure2026!
```

Avoid passwords such as:

```text
admin
password
12345678
router123
```

---

# 🛡️ Best Practices

When managing router passwords:

- Change the default administrator password immediately after installation.
- Use a unique password that is different from the Wi-Fi password.
- Store the password securely using a password manager or another secure method.
- Do not share administrator credentials unnecessarily.
- Change the password if unauthorized access is suspected.
- Keep the router firmware updated.

---

# 📷 Diagram

![change-the-default-administrator](https://github.com/varun-kumar-sec/networking-notes/blob/main/Working%20with%20Networking%20Devices/Image/Change-the-default-administrator-password.png?raw=true)

---

# 🎤 Interview Questions

### Beginner

- Why should the default administrator password be changed?
- Is the administrator password the same as the Wi-Fi password?
- What makes a strong administrator password?
- When should the administrator password be changed?

### Intermediate

- Explain the steps involved in changing the administrator password.
- What risks exist if the default password is not changed?
- Why should administrator and Wi-Fi passwords be different?
- List five best practices for securing router administrator access.

---

# 📌 Key Takeaways

- Default administrator passwords should always be changed after installing a router.
- The administrator password protects access to the router's management interface.
- A strong password should be long, unique, and difficult to guess.
- The administrator password and Wi-Fi password serve different purposes.
- Proper password management is a fundamental part of securing a network.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- Cisco Small Business Router Documentation
- TP-Link Support Documentation
- Microsoft Security Best Practices
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
