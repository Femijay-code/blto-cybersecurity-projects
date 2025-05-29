#  Sysmon Log Collection & Event Detection on Windows

This project focuses on collecting and detecting system-level events using Sysmon (System Monitor) on a Windows machine. It's designed to simulate a basic endpoint detection setup as part of my Blue Team Level One (BLTO) training.

---

##  Setup Overview

- **Tool Used**: Sysmon64.exe
- **Configuration Source**: Modified version of [SwiftOnSecurity's Sysmon config](https://github.com/SwiftOnSecurity/sysmon-config)
- **Host System**: Windows 10 (Intel Core i5-7200U, 8GB RAM)

---

##  Monitored Event IDs

| Event ID | Description               | Action Performed                              | Screenshot                        |
|----------|---------------------------|-----------------------------------------------|------------------------------------|
| 1        | Process Creation          | Opened Notepad and saved a file               | `event-id-1-process-create.png`    |
| 3        | Network Connection        | Visited a webpage (example.com)               | `event-id-3-network-connect.png`   |
| 11       | File Creation             | Created a new text file on desktop            | `event-id-11-file-create.png`      |
| 7        | Image Load                | Opened apps like Paint, Calculator            | `event-id-7-image-load.png`        |

---

##  Execution Steps

1. Installed Sysmon using:
   ```powershell
   .\Sysmon64.exe -accepteula -i sysmonconfig-export.xml


2. Modified the default config to enable monitoring for Event ID 1, 3, 7, and 11.

3. Triggered real activity to simulate endpoint behavior:

Opened apps

Created files

Made network requests

4. Verified logs in Event Viewer under:
   Applications and Services Logs > Microsoft > Windows > Sysmon > Operational
   
## 🖼️ Screenshots
    event-id-1-process-create.png

    event-id-3-network-connect.png

    event-id-11-file-create.png

    event-id-7-image-load.png
    
## Summary
This project simulates real-world endpoint monitoring using Sysmon. It builds the foundation for further detection engineering and SIEM pipeline development. All configurations, screenshots, and results are included in this folder.



