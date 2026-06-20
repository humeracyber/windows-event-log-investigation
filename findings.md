# Findings & Learning Summary

## Project Summary

This project involved investigating Windows Security Event Logs using Event Viewer to understand how authentication and system activity is recorded in Windows.

---

## Key Observations

- Successfully identified *Event ID 4624 (Successful Logon)*.
- Observed multiple logon types:
  - Logon Type 5 → Service Logon (background system activity)
  - Logon Type 7 → Unlock Workstation (user resumed session)
- Identified *Event ID 4634 (Logoff)* with Logon Type 2 (Interactive logoff).
- No suspicious or malicious activity was observed in the system logs.

---

## Important Learnings

- Windows logs are essential for tracking user and system activity.
- Different Logon Types represent different authentication methods.
- Not all security events indicate attacks — most are normal system behavior.
- SOC analysts must differentiate between normal and suspicious events.

---

## Challenges Faced

- Initially difficult to understand Event IDs and Logon Types.
- Some Event IDs (like 4625, 4720, 1102) were not present in the system.
- Learned that absence of events is also a valid finding in SOC analysis.

---

## Skills Gained

- Windows Event Viewer navigation
- Security log interpretation
- Logon type analysis
- Basic SOC investigation workflow
- Documentation of security findings

---

## Conclusion

This project provided hands-on experience in Windows log analysis. It helped build foundational SOC analyst skills such as identifying authentication events, understanding system activity, and documenting security investigations in a structured format.
