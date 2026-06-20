# Windows Event ID Reference Guide

This document explains important Windows Security Event IDs used in SOC (Security Operations Center) analysis.

---

## Authentication Events

### Event ID 4624 – Successful Logon
- Triggered when a user successfully logs into the system.
- Can include interactive, network, or service logons.
- Important for tracking legitimate access.

---

### Event ID 4625 – Failed Logon
- Triggered when a login attempt fails.
- Common causes: wrong password, locked account, or brute-force attempts.
- Important for detecting attacks.

---

### Event ID 4634 – Logoff
- Indicates a user session has ended.
- Helps correlate login duration with activity.

---

### Event ID 4648 – Explicit Credential Logon
- Occurs when a user logs in using different credentials.
- Can indicate lateral movement attempts.

---

## Privilege & Account Events

### Event ID 4672 – Special Privileges Assigned
- Indicates admin-level privileges assigned to a user.
- Important for privilege escalation detection.

---

### Event ID 4720 – User Account Created
- A new user account was created.
- Can be suspicious if unexpected.

---

### Event ID 4726 – User Account Deleted
- A user account was removed.
- Can indicate malicious cleanup activity.

---

## Process Events

### Event ID 4688 – Process Creation
- A new process has started.
- Useful for detecting malware or suspicious execution.

---

### Event ID 4689 – Process Termination
- A process has ended.
- Helps in tracking process lifecycle.

---

## Security Events

### Event ID 1102 – Security Log Cleared
- Indicates Windows event logs were cleared.
- Highly suspicious in security investigations.

---

## Summary

These Event IDs are commonly used by SOC analysts to:
- Detect suspicious logins
- Monitor user activity
- Track privilege changes
- Identify malicious behavior
