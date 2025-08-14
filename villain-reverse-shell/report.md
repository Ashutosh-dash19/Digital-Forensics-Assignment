# Villain Framework Reverse Shell Report

## ⚙️ Setup Info
- **Payload:** `windows/reverse_tcp/powershell`
- **LHOST:** 192.168.56.11
- **LPORT:** 8080

## 🔁 Payload Delivery Method
The payload was generated in Villain using the command:


It was then copied and executed in PowerShell on the Windows 10 target VM (running on the same internal VirtualBox network as the Kali attacker VM).

## 🖥️ Captured Info
- **Hostname:** <Captured from `systeminfo`>
- **IP Address:** <Captured from `ipconfig`>
- **User:** <Captured from `whoami`>

## Screenshots
- ![Villain access Screenshot](screenshots/Screenshot%201.png)
- ![Payload generation in linux](screenshots/Screenshot%202.png)
- ![Payload testing in windows](screenshots/Screenshot%203.png)
- ![Executing Commands](screenshots/Screenshot%204.png)
- ![System info windows 1](screenshots/Screenshot%205.png)
- ![System info windows 2](screenshots/Screenshot%206.png)

## 🔎 Enumeration Performed
```powershell
whoami
ipconfig
systeminfo

# Checking current user
whoami
# Output: WIN10LAB\Student

# Checking network configuration
ipconfig
# Output: IPv4 Address. . . . . . . . . . . : 192.168.56.1

# Gathering system information
systeminfo
# Output: Hostname: WIN10LAB
#         OS Name: Microsoft Windows 10 Pro
#         OS Version: 10.0.19045 N/A Build 19045





