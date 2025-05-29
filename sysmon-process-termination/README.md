# Sysmon Event ID 5 - Process Termination

This project documents how Sysmon logs process termination using Event ID 5. Tracking terminated processes can help correlate suspicious activity, especially when paired with process creation logs (Event ID 1) or parent-child process analysis.

---

## Summary

- Logged Event ID: **5** (Process Termination)
- Triggered by launching and terminating `notepad.exe` and `calc.exe`.
- Log entries show process name, ID, and termination time.
- Useful for tracing attacker cleanup, script self-deletion, or rapid execution chains.

---

## Tools Used

- Sysmon with `sysmonconfig-corrected.xml`
- Windows Event Viewer
- PowerShell

---

## Screenshots

| Description | Screenshot |
|-------------|------------|
| Notepad termination | ![eventid5-notepad](./eventid5-notepad.png) |
| Calculator termination | ![eventid5-calc](./eventid5-calc.png) |

