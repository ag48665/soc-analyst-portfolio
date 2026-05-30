# Windows Event Investigation

## Event ID 4624

### Description

Successful account logon.

### Event Details

- Event ID: 4624
- Category: Logon
- Result: Audit Success

### Analysis

A successful authentication event was identified in the Windows Security log.

### Skills Demonstrated

- Windows Event Viewer
- Security Log Analysis
- Authentication Monitoring


---

## Event ID 4625

### Description

Failed account logon.

### Event Details

- Event ID: 4625
- Category: Logon
- Result: Audit Failure
- Account Name: Agata
- Logon Type: 2 (Interactive Logon)

### Analysis

A failed authentication attempt was detected in the Windows Security log.

The investigation identified an invalid password entered during an interactive logon attempt.

### Findings

- Failure Reason: Unknown user name or bad password
- Status: 0xC000006D
- Sub Status: 0xC000006A (Wrong Password)
- Source Address: 127.0.0.1

### Security Relevance

This event type is commonly monitored to detect:

- Brute Force Attacks
- Password Spraying
- Unauthorized Access Attempts

### MITRE ATT&CK

T1110 - Brute Force

### Skills Demonstrated

- Event Viewer Analysis
- Authentication Monitoring
- Windows Security Logs

---















