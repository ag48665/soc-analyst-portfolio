# PowerShell Execution Detection Using Sysmon

## Objective

Detect PowerShell execution activity using Sysmon telemetry.

## Event Information

- Event ID: 1
- Event Type: Process Create
- User: Agata
- Process: powershell.exe

## Evidence

Sysmon recorded the creation of:

C:\Windows\System32\WindowsPowerShell\v1.0\powershell.exe

## Analysis

The process creation event confirms that PowerShell was executed on the host.

Sysmon captured:

- Process path
- Command line
- User context
- Process ID
- Logon session

This telemetry is frequently used by SOC analysts during threat hunting and incident investigations.

## Security Relevance

PowerShell is commonly abused by attackers for:

- Malware execution
- Script execution
- Download cradles
- Credential theft
- Lateral movement

## MITRE ATT&CK

T1059.001 - PowerShell

## Skills Demonstrated

- Sysmon
- Process Monitoring
- Windows Logging
- Threat Hunting
- Event Analysis
