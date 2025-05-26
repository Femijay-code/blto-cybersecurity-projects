# 🛡️ Blue Team Cybersecurity Projects

This repository features hands-on projects in network monitoring and intrusion detection, with a focus on endpoint visibility, system logging, and event correlation. Each folder documents a specific implementation with supporting artifacts.

---

##  Projects

### [Sysmon Log Collection on Windows](./sysmon-log-collection-windows)
Configured and deployed Sysmon for detailed Windows telemetry, capturing logs for process creation, driver loading, and network activity. Filtered and validated logs via Event Viewer for security-relevant event IDs.

 Tools: Sysmon, Event Viewer  
 Focus: Endpoint Monitoring, Log Collection


 ### [Windows Event Log Monitoring](./windows-event-log-monitoring)
Focused on detecting security-relevant Event IDs such as 4624 (logon), 4672/4673 (privilege use), and 4697 (service install) using native Windows Event Viewer. Includes log screenshots and detection summaries.


### [Event ID 13 - Registry Value Set](./Event-ID-13-Registry-Value-Set)  
Simulated and analyzed Event ID 13 to detect registry value changes, often linked to persistence techniques. Captured Sysmon logs and validated entries via Event Viewer.

**Tools:** Sysmon, Event Viewer  
**Focus:** Registry Monitoring, Persistence Detection

### [Process Termination - Sysmon Event ID 5](./process-termination-sysmon)
Logged and analyzed terminated processes using Sysmon’s Event ID 5. Useful for detecting attacker cleanup, terminated scripts, or suspicious parent-child process chains.

Tools: Sysmon, Event Viewer  
Focus: Process Monitoring, Endpoint Visibility



---
