# PowerShell Discovery Activity Detection

## Objective

Detect discovery activity launched from PowerShell using Sysmon telemetry.

## Event Information

| Field | Value |
|---------|---------|
| Event ID | 1 |
| Process | whoami.exe |
| Parent Process | powershell.exe |
| User | Agata |

## Analysis

Sysmon recorded the execution of whoami.exe from a PowerShell session.

The parent-child relationship identified:

- Parent Process: powershell.exe
- Child Process: whoami.exe

This activity is commonly observed during system discovery performed by administrators or threat actors.

## Evidence

![Whoami Execution](screenshots/whoami-from-powershell.png)

## Security Relevance

Threat actors frequently execute discovery commands to gather information about the environment.

Examples include:

- whoami
- hostname
- ipconfig
- net user

## MITRE ATT&CK

- T1033 – System Owner/User Discovery
- T1059.001 – PowerShell

## Skills Demonstrated

- Sysmon Analysis
- Threat Hunting
- Process Tree Analysis
- Windows Logging
