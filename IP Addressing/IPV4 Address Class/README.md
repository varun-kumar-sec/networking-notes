# IPv4 Address Classes
# 📖 Overview

When IPv4 was first introduced, addresses were divided into different **classes**. Each class was designed for networks of different sizes by allocating a different number of bits for the network and host portions of the address.

This system is known as **Classful Addressing**.

Although modern networks mainly use **CIDR (Classless Inter-Domain Routing)**, understanding IPv4 address classes remains important because they are frequently discussed in networking courses, certifications, and interviews.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What are IPv4 address classes?
- Why address classes were created
- Types of IPv4 address classes
- Network and host portions
- Uses of each address class
- Advantages and limitations of classful addressing

---

# 📑 Table of Contents

- What are IPv4 Address Classes?
- Why were Address Classes Created?
- Types of IPv4 Address Classes
- Class A
- Class B
- Class C
- Class D
- Class E
- Classful Addressing vs CIDR
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What are IPv4 Address Classes?

IPv4 addresses were originally divided into **five classes**:

- Class A
- Class B
- Class C
- Class D
- Class E

Each class supports different network sizes by allocating a different number of bits to the network and host portions.

---

# ❓ Why were Address Classes Created?

Address classes were introduced to:

- Support networks of different sizes.
- Simplify address allocation.
- Reduce address wastage.
- Organize IPv4 address assignments.

---

# 🅰️ Class A

### Range

```text
1.0.0.0
to
126.255.255.255
```

### First Bit

```text
0
```

### Default Subnet Mask

```text
255.0.0.0
```

### Network / Host

```text
Network : 8 bits
Host    : 24 bits
```

### Suitable For

- Very large organizations
- Large ISPs

---

# 🅱️ Class B

### Range

```text
128.0.0.0
to
191.255.255.255
```

### First Bits

```text
10
```

### Default Subnet Mask

```text
255.255.0.0
```

### Network / Host

```text
Network : 16 bits
Host    : 16 bits
```

### Suitable For

- Universities
- Medium-sized organizations

---

# 🅲 Class C

### Range

```text
192.0.0.0
to
223.255.255.255
```

### First Bits

```text
110
```

### Default Subnet Mask

```text
255.255.255.0
```

### Network / Host

```text
Network : 24 bits
Host    : 8 bits
```

### Suitable For

- Small businesses
- Home networks
- Small offices

---

# 🅳 Class D

### Range

```text
224.0.0.0
to
239.255.255.255
```

### Purpose

Used for **Multicast Communication**.

These addresses are **not assigned to individual hosts**.

---

# 🅴 Class E

### Range

```text
240.0.0.0
to
255.255.255.255
```

### Purpose

Reserved for:

- Experimental use
- Research

They are **not used for normal host addressing**.

---

# 📊 Summary Table

| Class | Address Range | Default Mask | Primary Use |
|------|----------------|--------------|-------------|
| A | 1.0.0.0 – 126.255.255.255 | 255.0.0.0 | Large Networks |
| B | 128.0.0.0 – 191.255.255.255 | 255.255.0.0 | Medium Networks |
| C | 192.0.0.0 – 223.255.255.255 | 255.255.255.0 | Small Networks |
| D | 224.0.0.0 – 239.255.255.255 | N/A | Multicast |
| E | 240.0.0.0 – 255.255.255.255 | N/A | Experimental |

---

# 📌 Classful Addressing vs CIDR

Originally, IPv4 addresses were allocated using fixed address classes.

Today, most networks use **CIDR (Classless Inter-Domain Routing)**, which allows more flexible address allocation and significantly reduces address wastage.

Even though CIDR has replaced classful addressing in modern networking, IPv4 classes are still important for learning networking fundamentals.

---

# 📷 Diagram

![Ipv4-address-classes](https://github.com/varun-kumar-sec/networking-notes/blob/main/IP%20Addressing/Image/IPv4-Address-Classes.png?raw=true)

---

# 🎤 Interview Questions

### Beginner

- What are IPv4 address classes?
- How many IPv4 address classes exist?
- Which class is used for multicast?
- Which class is used for experimental purposes?

### Intermediate

- Explain the difference between Class A, B, and C.
- Why were IPv4 address classes created?
- Why is classful addressing no longer commonly used?
- What replaced classful addressing?

---

# 📌 Key Takeaways

- IPv4 addresses were originally divided into **five classes**.
- Class A supports large networks.
- Class B supports medium-sized networks.
- Class C supports small networks.
- Class D is reserved for multicast communication.
- Class E is reserved for experimental use.
- Modern networks primarily use **CIDR**, but understanding IPv4 classes remains important for networking education and certifications.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- RFC 791 – Internet Protocol (IPv4)
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
