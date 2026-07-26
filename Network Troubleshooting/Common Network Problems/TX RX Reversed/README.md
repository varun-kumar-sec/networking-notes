# TX/RX Reversed
# 📖 Overview

**TX/RX Reversed** is a physical layer network problem that occurs when the **Transmit (TX)** and **Receive (RX)** wire pairs are connected incorrectly.

For successful Ethernet communication, the transmitting wires of one device must connect to the receiving wires of the other device. If these pairs are reversed incorrectly, devices cannot exchange data, resulting in communication failure.

This issue is commonly caused by incorrect cable termination or improper wiring during cable installation.

---

# 🎯 Learning Objectives

After completing this topic, you will be able to:

- Understand what TX/RX Reversed means.
- Explain why TX and RX pairs are important.
- Identify the causes of TX/RX reversal.
- Recognize common symptoms.
- Diagnose and resolve the problem.
- Apply preventive measures.

---

# 📑 Table of Contents

- What is TX/RX Reversed?
- Why TX and RX Pairs Matter
- Common Causes
- Symptoms
- How to Identify the Problem
- How to Fix the Problem
- Prevention
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is TX/RX Reversed?

In Ethernet communication:

- **TX (Transmit)** wires send data.
- **RX (Receive)** wires receive data.

For communication to work properly:

- TX on one device must connect to RX on the other device.

When TX is incorrectly connected to TX, or RX to RX, communication cannot be established.

---

# 🔄 Why TX and RX Pairs Matter

Ethernet devices communicate by transmitting and receiving data simultaneously.

Correct wiring ensures that:

- Data transmitted by one device is received by the other.
- Both devices can exchange information correctly.

If the transmit and receive pairs are incorrectly connected, the communication path is broken.

---

# ⚠️ Common Causes

TX/RX reversal is commonly caused by:

- Incorrect cable termination.
- Wiring errors during RJ-45 connector installation.
- Incorrect use of wiring standards.
- Improper cable repairs.
- Human error while crimping Ethernet cables.

---

# 🔍 Symptoms

Common symptoms include:

- No network connectivity.
- Link LEDs remain off.
- Devices fail to communicate.
- Unable to obtain an IP address.
- Ping requests fail.
- Network interface reports "Cable Unplugged" on some devices.

---

# 🛠️ How to Identify the Problem

### Cable Tester

A cable tester can identify:

- Reversed wire pairs.
- Crossed wire pairs.
- Incorrect cable termination.

---

### Visual Inspection

Verify that both cable ends follow the required wiring standard (T568A or T568B).

---

### Test with a Known Good Cable

Replace the suspected cable.

If communication is restored, the original cable is likely wired incorrectly.

---

# 🔧 How to Fix the Problem

To resolve TX/RX reversal:

1. Inspect both RJ-45 connectors.
2. Verify the wiring sequence.
3. Remove incorrectly terminated connectors.
4. Re-terminate the cable using the correct wiring standard.
5. Test the cable using a cable tester.
6. Verify network connectivity.

---

# 🛡️ Prevention

Prevent TX/RX reversal by:

- Following T568A or T568B consistently.
- Checking wire placement before crimping.
- Testing every newly created cable.
- Using quality crimping tools.
- Labeling tested cables.

---

# 🎤 Interview Questions

### Beginner

- What does TX stand for?
- What does RX stand for?
- Why must TX connect to RX?
- What happens if TX is connected to TX?

### Intermediate

- Explain the TX/RX reversal problem.
- What tool is commonly used to detect reversed wire pairs?
- What symptoms indicate a TX/RX reversal?
- How can this problem be prevented during cable installation?

---

# 📌 Key Takeaways

- TX represents **Transmit**, while RX represents **Receive**.
- Ethernet communication requires TX to connect to RX.
- Incorrect TX/RX connections prevent network communication.
- Cable testers quickly detect reversed wire pairs.
- Proper cable termination and testing prevent TX/RX reversal.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- TIA/EIA-568 Cabling Standard
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
