#  Windows Event Log Monitoring

This project focuses on collecting and analyzing Windows Security Event Logs to identify critical activities associated with logon events, service installations, and privilege escalations.

---

##  Event IDs Monitored

| Event ID | Description |
|----------|-------------|
| 4624     | Successful Logon |
| 4672     | Privileged Logon (Admin/Service Accounts) |
| 4673     | Sensitive Privilege Use Attempt |
| 4697     | New Service Installation |

---

##  Tools Used

- **Event Viewer** (Windows built-in)
- **Sysmon** (installed earlier but not used for this specific log set)

---

##  Key Findings

- **4624** logs show account logins including system services and local sessions.
- **4672** and **4673** confirm elevated privileges used, helping detect admin activity.
- **4697** was triggered by simulating service creation using PowerShell.
- Attempts to capture **7045 (New Service Installed)** was unsuccessful due to system configuration or audit policy gaps.

---

##  Screenshots

- `4624_successful_logon.png`
- `4672_privileged_logon.png`
- `4673_sensitive_privilege_use.png`
- `4697_service_installation.png`
- `filtered_event_view.png`

---

##  Summary

Monitoring Windows Security Event Logs is crucial for early threat detection, auditing user behavior, and uncovering unauthorized access attempts. This project simulates a practical approach to log collection and threat hunting using native Windows tools.
