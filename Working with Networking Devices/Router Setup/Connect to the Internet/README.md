# Connect to the Internet
# 📖 Overview

After placing the router in an appropriate location, the next step is to connect it to the Internet. This involves connecting the router to the Internet Service Provider (ISP) through a modem or an Ethernet connection, depending on the type of Internet service.

A properly connected router enables devices on the local network to access websites, online services, cloud applications, and other Internet resources.

---

# 🎯 Learning Objectives

After completing this topic, you will be able to:

- Understand how a router connects to the Internet.
- Identify the equipment required for an Internet connection.
- Connect a router to a modem or ISP.
- Verify Internet connectivity.
- Troubleshoot basic connection problems.

---

# 📑 Table of Contents

- Internet Connection Requirements
- Steps to Connect a Router to the Internet
- Verify the Connection
- Common Connection Problems
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 Internet Connection Requirements

To connect a router to the Internet, you typically need:

- A router.
- A modem (for cable, DSL, or fiber Internet) if required by the ISP.
- An active Internet service from an ISP.
- An Ethernet cable.
- A computer or mobile device for router configuration.

> **Note:** Some modern devices combine the modem and router into a single unit.

---

# 🛠️ Steps to Connect the Router

## Step 1: Turn Off the Devices

Before making cable connections:

- Turn off the modem.
- Turn off the router.

This helps ensure the devices initialize correctly after installation.

---

## Step 2: Connect the Modem to the Router

Use an Ethernet cable to connect:

```text
Modem LAN Port
        │
        ▼
Router WAN / Internet Port
```

The **WAN (Wide Area Network)** or **Internet** port is usually separate from the LAN ports and may be labeled or color-coded.

---

## Step 3: Power On the Modem

Turn on the modem first.

Wait until the modem's status indicators show that it has successfully connected to the ISP.

---

## Step 4: Power On the Router

After the modem is fully operational:

- Turn on the router.
- Wait for the router to complete its startup process.

The router should establish a connection with the modem.

---

## Step 5: Connect a Computer

Connect a computer:

- Using an Ethernet cable to a LAN port, **or**
- Through the router's Wi-Fi network.

This allows you to configure the router if necessary.

---

## Step 6: Configure Internet Settings (If Required)

Some ISPs automatically provide network settings using **DHCP**.

Others may require:

- PPPoE username and password.
- Static IP configuration.
- VLAN settings (depending on the ISP).

Enter the required information through the router's web management interface if prompted.

---

# ✅ Verify the Connection

After setup, verify that:

- The router's **Internet/WAN** indicator is active.
- Connected devices receive an IP address.
- A web browser can access websites.
- Internet services function normally.

You can also use troubleshooting tools such as:

- **Ping**
- **IPConfig**
- **Tracert**

to confirm connectivity.

---

# ⚠️ Common Connection Problems

## Loose Cable Connections

Ensure all Ethernet cables are securely connected.

---

## Incorrect Port

Verify that the modem is connected to the router's **WAN/Internet** port rather than a LAN port.

---

## Modem Not Connected

Confirm that the modem has established a connection with the ISP before turning on the router.

---

## Incorrect ISP Settings

If your ISP requires manual configuration, verify that the correct credentials and network settings have been entered.

---

## Internet Service Outage

If everything is configured correctly but Internet access is unavailable, check whether your ISP is experiencing a service outage.

---

# 📷 Diagram

Save the diagram as:

```text
images/connect-router-to-internet.png
```

Recommended diagram:

```text
        Internet
            │
            ▼
       +-----------+
       |   Modem   |
       +-----+-----+
             │
      Ethernet Cable
             │
             ▼
       +-----------+
       |  Router   |
       +-----+-----+
             │
     ┌───────┼────────┐
     ▼       ▼        ▼
   PC      Laptop   Smartphone
```

Suggested sources:

- https://www.cisco.com/
- https://support.google.com/
- https://www.tp-link.com/

---

# 🎤 Interview Questions

### Beginner

- What device usually connects the router to the ISP?
- Which router port is used for the Internet connection?
- Why should the modem be powered on before the router?
- How can you verify that the Internet connection is working?

### Intermediate

- Explain the steps involved in connecting a router to the Internet.
- What Internet settings might an ISP require?
- What happens if the modem is connected to a LAN port instead of the WAN port?
- How would you troubleshoot a router that cannot access the Internet?

---

# 📌 Key Takeaways

- A router connects to the Internet through a modem or directly to an ISP, depending on the connection type.
- The modem should be connected to the router's **WAN/Internet** port.
- Power on the modem before powering on the router.
- Some ISPs automatically configure the connection, while others require manual settings.
- After setup, always verify Internet connectivity and troubleshoot any issues before connecting additional devices.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- Cisco Documentation – Small Business Routers
- TP-Link Support Documentation
- Google WiFi Help Center
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
