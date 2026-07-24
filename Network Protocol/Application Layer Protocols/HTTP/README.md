# Hypertext Transfer Protocol (HTTP)
# 📖 Overview

The **Hypertext Transfer Protocol (HTTP)** is an application-layer protocol used for transferring web pages and other web resources between a web browser (client) and a web server.

HTTP follows a **client-server model**, where the client sends a request and the server responds with the requested resource.

It is the foundation of the **World Wide Web (WWW)** and enables users to browse websites using web browsers.

---

# 🎯 Learning Objectives

After completing this topic, you will understand:

- What is HTTP?
- Why HTTP is used
- How HTTP works
- HTTP request and response
- Common HTTP methods
- Advantages and limitations
- Real-world applications

---

# 📑 Table of Contents

- What is HTTP?
- Why is HTTP Needed?
- How HTTP Works
- HTTP Request and Response
- HTTP Methods
- Default Port
- Advantages
- Limitations
- Real-World Applications
- Diagram
- Interview Questions
- Key Takeaways
- References

---

# 🌐 What is HTTP?

**HTTP (Hypertext Transfer Protocol)** is a communication protocol used to transfer web pages, images, videos, documents, and other web content over the Internet.

Whenever you open a website in a browser, HTTP is used to exchange information between your browser and the web server.

Example:

```text
Browser  ───── HTTP Request ─────► Web Server
Browser ◄──── HTTP Response ───── Web Server
```

---

# ❓ Why is HTTP Needed?

HTTP is important because it:

- Enables web browsing.
- Allows browsers and web servers to communicate.
- Transfers web resources.
- Supports client-server communication.
- Forms the foundation of the World Wide Web.

---

# ⚙️ How HTTP Works

HTTP follows a simple **Request–Response** model.

### Step 1

A user enters a website address into a web browser.

↓

### Step 2

The browser sends an **HTTP Request** to the web server.

↓

### Step 3

The web server processes the request.

↓

### Step 4

The server returns an **HTTP Response** containing the requested resource.

↓

### Step 5

The browser displays the webpage to the user.

---

# 📨 HTTP Request and Response

## HTTP Request

A request sent by the client to ask for a resource.

Example:

- Request a webpage
- Submit a form
- Upload data

---

## HTTP Response

A response sent by the server containing:

- Status Code
- Headers
- Requested Content

Example:

```text
HTTP/1.1 200 OK
```

This indicates that the request was successful.

---

# 🛠️ Common HTTP Methods

| Method | Purpose |
|---------|----------|
| GET | Retrieve data from the server |
| POST | Send data to the server |
| PUT | Update existing data |
| DELETE | Remove data from the server |

---

# 📡 Default Port

| Protocol | Port |
|----------|-----:|
| HTTP | TCP 80 |

---

# ✅ Advantages

- Simple and easy to implement.
- Widely supported.
- Fast communication.
- Supports multimedia content.
- Foundation of the World Wide Web.

---

# ❌ Limitations

- Data is transmitted in plain text.
- No encryption.
- Vulnerable to interception and modification.
- Not suitable for transmitting sensitive information.

> **Note:** Secure web communication is provided by **HTTPS**, which encrypts HTTP traffic using TLS/SSL.

---

# 🌍 Real-World Applications

HTTP is used in:

- Web browsing
- Web applications
- REST APIs
- Online documentation
- Content delivery
- Web services

---

# 📷 Diagram

![HTTP](https://github.com/varun-kumar-sec/networking-notes/blob/main/Network%20Protocol/Image/HTTP.png?raw=true)

---

# 🎤 Interview Questions

### Beginner

- What is HTTP?
- Which port does HTTP use?
- What is the purpose of HTTP?
- What communication model does HTTP use?

### Intermediate

- Explain the HTTP request-response process.
- Differentiate between an HTTP request and an HTTP response.
- Explain the purpose of GET and POST methods.
- Why is HTTP considered insecure?

---

# 📌 Key Takeaways

- HTTP stands for **Hypertext Transfer Protocol**.
- It is used for communication between web browsers and web servers.
- HTTP follows a **client-server request-response model**.
- HTTP uses **TCP Port 80**.
- Common methods include **GET, POST, PUT, and DELETE**.
- Because HTTP does not encrypt data, sensitive communication should use **HTTPS**.

---

# 📚 References

- Cisco Networking Academy (NetAcad)
- CompTIA Network+
- RFC 9110 – HTTP Semantics
- RFC 9112 – HTTP/1.1
- Andrew S. Tanenbaum – *Computer Networks*
- Behrouz A. Forouzan – *Data Communications and Networking*
