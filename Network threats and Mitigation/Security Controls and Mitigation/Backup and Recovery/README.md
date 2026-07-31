# Backup and Recovery
# 📖 Overview

**Backup and Recovery** are security and business-continuity practices used to protect data and restore systems after data loss, hardware failure, malware infection, ransomware, accidental deletion, or other incidents.

A **backup** is a separate copy of data, while **recovery** is the process of restoring data or systems to a usable state.

```text
Important Data
     │
     ▼
   Backup
     │
     ▼
Separate Storage
     │
     │  Incident
     ▼
Recovery Process
     │
     ▼
Restored Data/System
```
---

# 🎯 Learning Objectives

After completing this section, you will be able to:

Understand backup and recovery.
Explain why backups are important.
Identify common backup types.
Understand the 3-2-1 backup strategy.
Understand Recovery Point Objective (RPO) and Recovery Time Objective (RTO).
Identify backup security best practices.
Explain basic recovery procedures.

---

# 📚 Topics Covered

This section includes:

What is a Backup?
What is Recovery?
Why Backups are Important
Types of Backups
3-2-1 Backup Strategy
RPO and RTO
Backup Storage
Backup Security
Recovery Process
Backup Testing
Real-World Applications

---

# 💾 What is a Backup?

A backup is a copy of important data stored separately from the original data.

Backups can protect against:

Accidental deletion
Hardware failure
Malware
Ransomware
Data corruption
Software failures
Theft
Natural disasters

A backup should be sufficiently isolated so that an incident affecting the original data does not automatically destroy the backup.

---

# 🔄 What is Recovery?

Recovery is the process of restoring data, applications, or systems after an incident.

Recovery may involve:

Restoring files
Restoring databases
Reinstalling operating systems
Restoring system configurations
Rebuilding servers
Recovering services
Incident
   │
   ▼
Assess Damage
   │
   ▼
Identify Clean Backup
   │
   ▼
Restore Data/System
   │
   ▼
Verify
   │
   ▼
Return to Operation

---

# 🧩 Types of Backups

| Backup Type             | Description                                                |
| ----------------------- | ---------------------------------------------------------- |
| **Full Backup**         | Copies all selected data.                                  |
| **Incremental Backup**  | Copies data changed since the previous backup of any type. |
| **Differential Backup** | Copies data changed since the last full backup.            |
| **Image Backup**        | Creates a complete image of a system, disk, or partition.  |

Comparison

| Type         | Backup Size             | Backup Speed | Recovery Complexity                                       |
| ------------ | ----------------------- | ------------ | --------------------------------------------------------- |
| Full         | Larger                  | Slower       | Usually simpler                                           |
| Incremental  | Smaller                 | Faster       | Can require multiple backup sets                          |
| Differential | Medium/Larger over time | Moderate     | Usually requires the full backup plus latest differential |

---

# 🔢 The 3-2-1 Backup Strategy

The 3-2-1 strategy is a common backup principle:

3 copies of important data.
Stored on at least 2 different types of storage/media.
At least 1 copy kept off-site.
              Important Data
                    │
        ┌───────────┼───────────┐
        ▼           ▼           ▼
     Primary     Backup 1     Backup 2
     Storage      Local       Off-site
                    │
                 Different
                 Storage

Modern environments may additionally use immutable or offline backups to improve protection against ransomware.

---

# ⏱️ RPO and RTO
Recovery Point Objective (RPO)

RPO defines how much data loss, measured in time, an organization is willing to tolerate.

Example:

An RPO of 1 hour means the organization aims to recover data to a point no more than approximately 1 hour before an incident.

Recovery Time Objective (RTO)

RTO defines how quickly a system or service should be restored after an incident.

Example:

An RTO of 4 hours means the organization aims to restore the service within approximately 4 hours.

| Term    | Meaning                                   |
| ------- | ----------------------------------------- |
| **RPO** | How much data loss is acceptable?         |
| **RTO** | How quickly must the service be restored? |

---

# ☁️ Backup Storage

Backups can be stored:

On external drives
On dedicated backup servers
On Network Attached Storage (NAS)
In cloud storage
At an off-site facility
On removable or offline media

Important backups should be protected from unauthorized access and accidental deletion.

---

# 🔐 Backup Security

Backups themselves contain valuable information and must be protected.

Organizations should:

Encrypt sensitive backups.
Restrict access to backup systems.
Use strong authentication and MFA.
Protect backup credentials.
Keep some backups offline or immutable.
Separate backup administration from normal user accounts.
Monitor backup activity.
Regularly test backups.
Protect backup infrastructure from ransomware.
Maintain appropriate retention policies.

---

# 🧪 Backup Testing

A backup is useful only if it can actually be restored.

Organizations should regularly perform restore tests to verify:

Backup integrity
Data completeness
Recovery procedures
Recovery time
Application functionality
Backup Created
      │
      ▼
Restore Test
      │
      ▼
Verify Data
      │
 ┌────┴────┐
 ▼         ▼
Success   Failure
 │           │
 ▼           ▼
Continue   Investigate
            & Fix

---
  
# 🚨 Recovery After Ransomware

If ransomware affects a system:

Isolate affected systems.
Prevent the malware from spreading.
Investigate the incident.
Identify clean backups.
Ensure the backup environment is not compromised.
Remove or remediate the infection.
Restore systems and data.
Apply required security updates.
Reset compromised credentials when necessary.
Monitor restored systems.

Do not assume that the newest backup is clean. Verify backups before restoring them.

---

# 🛡️ Backup Best Practices

Organizations should:

Back up critical data regularly.
Automate backups where appropriate.
Use multiple backup locations.
Maintain offline or immutable copies.
Encrypt sensitive backups.
Test restoration regularly.
Define retention periods.
Monitor backup jobs for failures.
Document recovery procedures.
Define RPO and RTO requirements.
Protect backup accounts with strong authentication.
Keep backup systems separated from ordinary user access.

---

# 💼 Real-World Applications

Backup and recovery are important in:

Businesses
Data centers
Cloud environments
Hospitals
Banks
Government organizations
Schools and universities
Personal computers
Servers
Network infrastructure

---

# 🛠️ Skills You'll Gain

After completing this section, you'll be able to:

Define backup and recovery.
Identify common backup types.
Explain the 3-2-1 backup strategy.
Understand RPO and RTO.
Identify secure backup-storage methods.
Explain why backup testing is important.
Understand basic ransomware recovery procedures.
Apply basic backup security best practices.

---

# 📌 Key Takeaways

A backup is a separate copy of data; recovery is the process of restoring data or systems.
Backups help protect against accidental deletion, hardware failure, malware, ransomware, corruption, and disasters.
Common backup types include full, incremental, differential, and image backups.
The 3-2-1 strategy recommends multiple copies, different storage types, and an off-site copy.
RPO defines acceptable data loss, while RTO defines the target recovery time.
Backups should be encrypted, access-controlled, monitored, and regularly tested.
Offline or immutable backups provide additional protection against ransomware.
A backup should never be considered reliable until a successful restore test has been performed.
Backup and recovery support Availability and help organizations maintain business continuity after security incidents.

---

# 📚 References

- NIST Cybersecurity Framework
- NIST SP 800-34 – Contingency Planning Guide
- CISA – Data Backup and Recovery Guidance
- Microsoft Learn – Backup and Recovery Documentation
- Cisco Networking Academy (NetAcad)
- CompTIA Security+
