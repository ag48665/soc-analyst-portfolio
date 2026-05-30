# Sysmon Process Creation Monitoring

## Objective

Monitor process creation events using Sysmon.

## Event Details

- Event ID: 1
- Event Type: Process Creation
- Process: notepad.exe
- Path: C:\Windows\System32\notepad.exe

## Analysis

Sysmon successfully detected the creation of a new process.

The event captured:

- Process Name
- Process Path
- Process ID
- Timestamp

## Security Relevance

Process creation monitoring is critical for detecting:

- Malware execution
- PowerShell abuse
- Suspicious command execution
- Living-off-the-Land techniques

## MITRE ATT&CK

T1059 - Command and Scripting Interpreter

## Skills Demonstrated

- Sysmon
- Event Analysis
- Threat Hunting
- Windows Monitoring
