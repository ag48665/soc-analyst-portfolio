# Scheduled Task Creation Detection

## Objective

Detect the creation of scheduled tasks using Windows Task Scheduler logs.

## Event Information

- Log Source: Microsoft-Windows-TaskScheduler/Operational
- Event ID: 106
- Task Name: TestTask2
- User: Agata

## Evidence

Task Scheduler recorded the registration of a new scheduled task.

Event Message:

User "DESKTOP-VL94PBM\Agata" registered Task Scheduler task "\TestTask2"

## Analysis

The event confirms that a new scheduled task was created on the host.

Scheduled tasks are frequently used by administrators for automation, but they are also abused by attackers to establish persistence.

## Security Relevance

Scheduled tasks can be used for:

- Persistence
- Malware Execution
- Privilege Escalation
- Automated Command Execution

## MITRE ATT&CK

T1053.005 - Scheduled Task

## Skills Demonstrated

- Windows Event Analysis
- Task Scheduler Monitoring
- Persistence Detection
- Threat Hunting
