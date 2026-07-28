# Save and Test the Configuration
# 📖 Overview

After configuring a router, the final step is to **save the configuration** and **test the network**. Saving ensures that all configuration changes are stored in the router's memory and remain active after a reboot. Testing verifies that the router and network are functioning as expected.

Skipping this step may result in lost configuration changes or unnoticed connectivity issues.

---

# 🎯 Learning Objectives

After completing this topic, you will be able to:

- Save router configuration changes.
- Verify that the router is operating correctly.
- Test Internet and local network connectivity.
- Confirm Wi-Fi functionality.
- Perform basic post-configuration checks.

---

# 📑 Table of Contents

- Why Save the Configuration?
- Steps to Save the Configuration
- Testing the Network
- Common Issues After Configuration
- Best Practices
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 💾 Why Save the Configuration?

Most routers require you to manually save or apply configuration changes.

Saving the configuration ensures that:

- New settings become active.
- Changes are retained after restarting the router.
- Configuration work is not lost.

Some routers automatically save settings, while others require selecting **Save**, **Apply**, or **Save Configuration**.

---

# 🛠️ Steps to Save the Configuration

## Step 1: Review Settings

Before saving, verify that the following settings are correct:

- Internet connection settings.
- LAN configuration.
- DHCP settings.
- Wi-Fi SSID.
- Wireless security mode.
- Wi-Fi password.
- Administrator password.

---

## Step 2: Save or Apply Changes

Click:

```text
Save
```

or

```text
Apply
```

depending on the router model.

Wait for the router to process the configuration. Some routers may briefly restart their network services.

---

## Step 3: Restart the Router (If Required)

Some routers require a reboot for certain configuration changes to take effect.

If prompted:

- Restart the router.
- Wait until all status indicators return to normal.

---

# ✅ Testing the Network

After saving the configuration, verify that everything works correctly.

## Check Internet Access

Open a web browser and visit several websites.

If pages load successfully, the router has Internet connectivity.

---

## Verify Wi-Fi Connectivity

Connect a wireless device using the configured:

- SSID
- Wi-Fi password

Ensure the device successfully joins the network.

---

## Verify IP Address Assignment

Confirm that connected devices receive a valid IP address from the router's DHCP server.

Example:

```text
IP Address: 192.168.1.100
Subnet Mask: 255.255.255.0
Default Gateway: 192.168.1.1
```

---

## Test Network Communication

Verify communication by:

- Opening websites.
- Accessing shared network devices.
- Using commands such as:

```text
ping
```

or

```text
ipconfig
```

to confirm network connectivity.

---

# ⚠️ Common Issues After Configuration

If testing fails, check for:

- Loose Ethernet cables.
- Incorrect WAN connection.
- Incorrect Wi-Fi password.
- Disabled DHCP service.
- Incorrect Internet settings.
- ISP connectivity issues.

Correct the problem and repeat the tests.

---

# 🛡️ Best Practices

After completing the configuration:

- Save all configuration changes.
- Test both wired and wireless connections.
- Verify Internet access on multiple devices.
- Record important network settings for future reference.
- Keep the router firmware updated.
- Regularly review the router's configuration and security settings.

---

# 📷 Diagram

Save the diagram as:

```text
images/save-and-test-configuration.png
```

Recommended diagram:

```text
Configure Router
        │
        ▼
Save / Apply Settings
        │
        ▼
Restart (if required)
        │
        ▼
Test Internet Connection
        │
        ▼
Test Wi-Fi Connection
        │
        ▼
Verify IP Address
        │
        ▼
Network Ready ✔
```

Suggested sources:

- https://www.cisco.com/
- https://support.google.com/
- https://www.tp-link.com/

---

# 🎤 Interview Questions

### Beginner

- Why should router configuration be saved?
- How can you verify that the Internet connection is working?
- Why should you test the Wi-Fi connection after configuration?
- What command can be used to test basic network connectivity?

### Intermediate

- Explain the steps involved in saving and testing a router configuration.
- What should you verify before saving the configuration?
- What common problems might occur after router configuration?
- Why is testing an important part of the router setup process?

---

# 📌 Key Takeaways

- Saving the configuration ensures that router settings are retained and applied correctly.
- Always verify Internet connectivity after configuration.
- Test both wired and wireless network connections.
- Confirm that connected devices receive valid IP addresses.
- Performing post-configuration testing helps identify and resolve issues before the network is put into regular use.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- Cisco Small Business Router Documentation
- TP-Link Support Documentation
- Microsoft Learn – Networking Documentation
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
