# IPv4 Binary to Decimal Conversion
# 📖 Overview

Although IPv4 addresses are commonly written in **decimal format**, computers store and process them in **binary (base-2)**.

Understanding how to convert between binary and decimal is essential because many networking concepts—such as subnetting, subnet masks, network IDs, and broadcast addresses—are based on binary calculations.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- Why binary is used in networking
- Binary number system
- Decimal number system
- Binary place values
- Binary to decimal conversion
- Decimal to binary conversion
- Converting an IPv4 address

---

# 📑 Table of Contents

- Why Binary is Used
- Decimal Number System
- Binary Number System
- Binary Place Values
- Binary to Decimal Conversion
- Decimal to Binary Conversion
- IPv4 Conversion Example
- Tips for Quick Conversion
- Interview Questions
- Key Takeaways
- References

---

# 💻 Why Binary is Used

Computers understand only two electrical states:

- ON
- OFF

These are represented as:

```text
ON  = 1
OFF = 0
```

Therefore, computers use the **Binary Number System (Base-2)**.

Humans, however, usually work with the **Decimal Number System (Base-10)**.

---

# 🔢 Decimal Number System

The decimal system contains ten digits.

```text
0 1 2 3 4 5 6 7 8 9
```

Example:

```text
356

= 3×100
+ 5×10
+ 6×1

= 356
```

---

# 🔢 Binary Number System

Binary contains only two digits.

```text
0
1
```

Example:

```text
10110110
```

Each digit is called a **bit**.

---

# 🏗️ Binary Place Values

An IPv4 octet contains **8 bits**.

Each bit has a fixed decimal value.

| Bit Position | 8 | 7 | 6 | 5 | 4 | 3 | 2 | 1 |
|--------------|---|---|---|---|---|---|---|---|
| Decimal Value |128|64|32|16|8|4|2|1|

Remember this table—it is used throughout networking.

---

# 🔄 Binary to Decimal Conversion

To convert binary into decimal:

1. Write the place values.
2. Ignore positions containing **0**.
3. Add the values where the bit is **1**.

Example:

```text
Binary

11000000

Place Values

128 64 32 16 8 4 2 1
 1   1  0  0 0 0 0 0

128 + 64

= 192
```

Another example:

```text
11111111

128+64+32+16+8+4+2+1

=255
```

---

# 🔄 Decimal to Binary Conversion

To convert decimal into binary:

1. Start with the largest place value.
2. If the value fits, write **1**.
3. Subtract it.
4. Continue until reaching 1.

Example:

Convert **192**

| Value |128|64|32|16|8|4|2|1|
|------:|--:|--:|--:|--:|--:|--:|--:|--:|
|Bit|1|1|0|0|0|0|0|0|

Result:

```text
192

↓

11000000
```

Example:

Convert **10**

```text
8 + 2

↓

00001010
```

---

# 🌐 IPv4 Conversion Example

IPv4 Address:

```text
192.168.1.10
```

Binary:

```text
11000000.10101000.00000001.00001010
```

Each decimal octet is converted separately.

---

# 💡 Tips for Quick Conversion

- Memorize the place values:

```text
128 64 32 16 8 4 2 1
```

- Maximum value:

```text
11111111 = 255
```

- Minimum value:

```text
00000000 = 0
```

- Every IPv4 octet always contains **8 bits**.

---

# 📷 Diagram

![ipv4-to-decimal-conversion](https://github.com/varun-kumar-sec/networking-notes/blob/main/IP%20Addressing/Image/ipv4-to-decimal-conversion.png?raw=true)

---

# 🎤 Interview Questions

### Beginner

- Why do computers use binary?
- How many bits are in one IPv4 octet?
- What is the decimal value of 11111111?
- What is the binary value of 255?

### Intermediate

- Convert 172 into binary.
- Convert 10101010 into decimal.
- Why is binary important in networking?
- Why must every IPv4 octet contain exactly 8 bits?

---

# 📌 Key Takeaways

- Computers process data using binary.
- Humans usually write IPv4 addresses in decimal.
- One IPv4 octet contains **8 bits**.
- Binary place values are:

```text
128 64 32 16 8 4 2 1
```

- Each octet ranges from **0 to 255**.
- Understanding binary conversion is essential for subnetting and advanced IP addressing topics.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
