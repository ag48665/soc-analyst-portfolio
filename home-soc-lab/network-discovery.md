# Network Discovery Activity Detection

## Objective

Investigate network discovery activity using Sysmon telemetry.

## Event Information

| Field | Value |
|---------|---------|
| Event ID | 1 |
| Process | ipconfig.exe |
| Parent Process | powershell.exe |
| User | Agata |

## Analysis

Sysmon recorded the execution of ipconfig.exe from a PowerShell session.

The activity was used to collect network configuration information from the host.

Parent-child relationship:

powershell.exe
└── ipconfig.exe

Sysmon captured:

- Process path
- Command line
- User context
- Parent process
- SHA256 hash

## Evidence

![Network Discovery](screenshots/network-discovery-ipconfig.png)

## Security Relevance

Attackers frequently perform network discovery to:

- Identify IP configuration
- Gather network information
- Enumerate host settings
- Prepare lateral movement

## MITRE ATT&CK

- T1016 – System Network Configuration Discovery

## Skills Demonstrated

- Sysmon Analysis
- Threat Hunting
- Network Discovery Analysis
- Windows Logging
