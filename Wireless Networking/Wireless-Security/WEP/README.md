# Wired Equivalent Privacy (WEP)
# 📖 Overview

**Wired Equivalent Privacy (WEP)** is one of the earliest security protocols developed to protect wireless networks.

Its goal was to provide a level of security for wireless networks comparable to that of traditional wired Ethernet networks. WEP encrypts data transmitted between wireless devices and the Wireless Access Point (WAP) to help prevent unauthorized access.

Although WEP was widely used in the early days of Wi-Fi, it is now considered **insecure** and has been replaced by stronger security protocols such as **WPA**, **WPA2**, and **WPA3**.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What is WEP?
- Why WEP was developed
- How WEP works
- Advantages and limitations
- Why WEP is no longer recommended

---

# 📑 Table of Contents

- What is WEP?
- Why WEP Was Developed
- How WEP Works
- Advantages
- Limitations
- Why WEP Became Obsolete
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is WEP?

**Wired Equivalent Privacy (WEP)** is a wireless security protocol designed to protect Wi-Fi networks by encrypting transmitted data.

Its primary objectives were:

- Prevent unauthorized network access.
- Protect wireless data from interception.
- Provide basic confidentiality for wireless communication.

---

# ❓ Why WEP Was Developed

Wireless communication uses radio waves, making it easier for nearby attackers to intercept transmitted data.

WEP was introduced to:

- Secure wireless communication.
- Reduce unauthorized access.
- Protect data exchanged over Wi-Fi networks.

---

# ⚙️ How WEP Works

WEP operates using a shared secret key.

The communication process is generally as follows:

1. A wireless device requests to join the network.
2. The device provides the correct WEP key.
3. The Access Point verifies the key.
4. Data is encrypted before transmission.
5. The receiving device decrypts the data using the same key.

Both the client and the access point must use the **same encryption key**.

---

# ✅ Advantages

- Easy to configure.
- Introduced basic wireless encryption.
- Reduced casual unauthorized access.
- Supported by early Wi-Fi equipment.

---

# ❌ Limitations

- Weak encryption algorithm.
- Vulnerable to key recovery attacks.
- Shared key management is difficult.
- Can be broken within a short period using modern attack tools.
- No longer considered secure.

---

# ⚠️ Why WEP Became Obsolete

Researchers discovered serious security weaknesses in WEP.

As computing power increased, attackers could recover WEP encryption keys relatively quickly.

Because of these vulnerabilities, WEP was replaced by:

- WPA
- WPA2
- WPA3

Today, WEP should **not** be used to secure wireless networks.

---

# 📷 Diagram

Save the diagram as:

```text
images/wep.png
```

Recommended diagram:

```text
Laptop
   │
Encrypted Data (WEP)
   │
~~~~~~~~ Wi-Fi Signal ~~~~~~~~
   │
Wireless Access Point
```

Suggested sources:

- https://commons.wikimedia.org/wiki/Category:Wireless_security
- https://en.wikipedia.org/wiki/Wired_Equivalent_Privacy

---

# 🎤 Interview Questions

### Beginner

- What does WEP stand for?
- Why was WEP developed?
- Does WEP encrypt wireless data?
- Is WEP considered secure today?

### Intermediate

- Explain how WEP works.
- Why is WEP vulnerable to attacks?
- What replaced WEP?
- Why should WEP not be used in modern wireless networks?

---

# 📌 Key Takeaways

- WEP stands for **Wired Equivalent Privacy**.
- It was the first widely used Wi-Fi security protocol.
- WEP encrypts wireless communication using a shared key.
- Serious security weaknesses make WEP unsafe today.
- Modern wireless networks should use **WPA2** or **WPA3** instead of WEP.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- IEEE 802.11 Wireless LAN Standards
- Wi-Fi Alliance
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
