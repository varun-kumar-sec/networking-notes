# Authentication and Access Control
# 📖 Overview

**Authentication** and **Access Control** are fundamental security mechanisms used to verify a user's identity and determine what resources they are allowed to access.

Authentication answers **"Who are you?"**, while Access Control answers **"What are you allowed to do?"**

Together, they help protect systems, applications, and data from unauthorized access.

```text
User
  │
  ▼
Authentication
(Verify Identity)
  │
  ▼
Access Control
(Check Permissions)
  │
  ▼
Allow or Deny Access
```

---

# 🎯 Learning Objectives

After completing this section, you will be able to:

- Understand authentication and access control.
- Differentiate authentication from authorization.
- Identify common authentication methods.
- Understand Multi-Factor Authentication (MFA).
- Understand access control models.
- Identify authentication and access control best practices.

---

# 📚 Topics Covered

This section includes:

- What is Authentication?
- Authentication Factors
- Multi-Factor Authentication (MFA)
- What is Access Control?
- Authentication vs Authorization
- Access Control Models
- Principle of Least Privilege
- Best Practices
- Real-World Applications

---

# 🔐 What is Authentication?

**Authentication** is the process of verifying the identity of a user, device, or service before granting access.

Common authentication methods include:

- Username and password
- PIN
- Smart card
- Security token
- Fingerprint
- Facial recognition
- One-Time Password (OTP)

---

# 🔑 Authentication Factors

Authentication factors are grouped into categories:

| Factor | Example |
|---|---|
| **Something You Know** | Password, PIN, Security Question |
| **Something You Have** | Smartphone, Smart Card, Hardware Token |
| **Something You Are** | Fingerprint, Face Recognition, Iris Scan |

Using multiple factors provides stronger security than relying on a password alone.

---

# 🛡️ Multi-Factor Authentication (MFA)

**MFA** requires two or more authentication factors before access is granted.

```text id="u7k2pr"
Username + Password
          │
          ▼
Authentication App / OTP
          │
          ▼
Access Granted
```

Benefits of MFA:

- Reduces account compromise.
- Protects against stolen passwords.
- Improves account security.
- Adds an additional verification layer.

---

# 🚪 What is Access Control?

**Access Control** determines what an authenticated user is allowed to access or perform.

Examples include:

- Reading files
- Modifying data
- Installing software
- Accessing network resources
- Managing systems

Possible permissions include:

- Read
- Write
- Execute
- Modify
- Delete
- Full Control

---

# ⚖️ Authentication vs Authorization

| Authentication | Authorization |
|---|---|
| Verifies identity. | Determines permissions. |
| Happens first. | Happens after authentication. |
| Answers **"Who are you?"** | Answers **"What can you access?"** |

---

# 🧩 Access Control Models

| Model | Description |
|---|---|
| **DAC (Discretionary Access Control)** | Resource owners determine who has access. |
| **MAC (Mandatory Access Control)** | Access is controlled using security classifications defined by the organization. |
| **RBAC (Role-Based Access Control)** | Permissions are assigned according to job roles. |
| **ABAC (Attribute-Based Access Control)** | Access decisions are based on attributes such as user, device, location, or time. |

---

# 🔒 Principle of Least Privilege

The **Principle of Least Privilege (PoLP)** means users should receive **only the permissions necessary** to perform their job.

```text id="p6d1tx"
User
 │
 ▼
Minimum Required Permissions
 │
 ▼
Reduced Security Risk
```

Benefits include:

- Reduced attack surface
- Reduced accidental changes
- Better protection of sensitive information
- Limited impact if an account is compromised

---

# 🛡️ Authentication and Access Control Best Practices

Organizations should:

- Use strong, unique passwords.
- Enable MFA.
- Apply least privilege.
- Use role-based access where appropriate.
- Disable unused accounts.
- Review permissions regularly.
- Remove unnecessary administrative privileges.
- Monitor login activity.
- Lock accounts after repeated failed login attempts.
- Keep authentication systems updated.

---

# 🚨 Responding to Unauthorized Access

If unauthorized access is suspected:

1. Lock or disable the affected account.
2. Reset compromised passwords.
3. Revoke active sessions.
4. Review authentication logs.
5. Investigate affected systems.
6. Re-enable MFA if disabled.
7. Review permissions and roles.
8. Report the incident to the security team.
9. Continue monitoring for suspicious activity.

---

# 💼 Real-World Applications

Authentication and Access Control are used in:

- Windows and Linux systems
- Active Directory
- Cloud platforms
- Corporate networks
- Banking systems
- Healthcare organizations
- Government agencies
- Web applications
- Remote-access VPNs
- Email systems

---

# 🛠️ Skills You'll Gain

After completing this section, you'll be able to:

- Define authentication and access control.
- Differentiate authentication from authorization.
- Identify authentication factors.
- Explain the importance of MFA.
- Understand common access control models.
- Apply the Principle of Least Privilege.
- Identify authentication and access control best practices.

---

# 📌 Key Takeaways

- **Authentication** verifies identity, while **Access Control** determines permissions.
- Authentication commonly uses **passwords, tokens, smart cards, OTPs, and biometrics**.
- **MFA** significantly improves account security by requiring multiple authentication factors.
- Common access control models include **DAC, MAC, RBAC, and ABAC**.
- The **Principle of Least Privilege** reduces security risks by granting only the minimum permissions required.
- Regular permission reviews, strong passwords, MFA, monitoring, and account management are essential for protecting systems and data.

---

# 📚 References

- NIST Cybersecurity Framework
- NIST SP 800-63 – Digital Identity Guidelines
- Microsoft Learn – Identity and Access Management
- Cisco Networking Academy (NetAcad)
- CompTIA Security+
