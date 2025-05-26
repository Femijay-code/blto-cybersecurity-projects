# Event ID 13 - Registry Value Set (Sysmon)

## 📝 Description
This project demonstrates the detection of Windows registry value changes using **Sysmon Event ID 13**. This type of event is critical for monitoring unauthorized changes to the system registry, which can be indicative of malware persistence or system misconfigurations.

## 🔧 Tools & Setup
- **Sysmon v15.15** (installed under `C:\Tools\Sysmon`)
- **Sysmon config:** `sysmonconfig-corrected.xml`
- **Event Viewer** (Windows Logs → Applications and Services Logs → Microsoft → Windows → Sysmon → Operational)

## ⚙️ Test Steps
1. Open PowerShell with Administrator privileges.
2. Run the following command to simulate a registry value change:

   ```powershell
   Set-ItemProperty -Path HKCU:\Software\Microsoft\Windows\CurrentVersion\Explorer -Name TestValue -Value "BLTOtest"
