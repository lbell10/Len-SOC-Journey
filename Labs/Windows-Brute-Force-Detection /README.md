# Windows Brute Force Detection Lab

## Objective
Simulate and detect a brute force authentication attack using Windows Security logs.

## Lab Environment
Host Machine: Windows 11 VM  
Logging Source: Windows Security Logs  
Monitoring Tool: Event Viewer  

## Attack Simulation
A brute force scenario was simulated by generating multiple failed login attempts using incorrect credentials.

Command used:

runas /user:Administrator cmd

Multiple incorrect passwords were entered to trigger failed authentication events.

## Detection Steps
1. Open Event Viewer
2. Navigate to:

Windows Logs → Security

3. Filter logs for Event ID:

4625

This event represents a failed logon attempt.

## Findings
Multiple Event ID 4625 entries were observed within a short timeframe, indicating repeated failed login attempts.

Key Event Details:

Event ID: 4625  
Task Category: Logon  
Log Level: Audit Failure  

Account Targeted: lenla  
Computer: WIN11-CLIENT01  

## Evidence

Screenshot of Event Viewer showing multiple failed login attempts:

![Brute Force Detection](Labs/Windows-Brute-Force-Detection/Screenshots/Brute-Force-4625.png)

## Conclusion
Repeated failed authentication attempts can indicate a brute force attack. Monitoring Event ID 4625 in Windows Security logs helps security analysts detect potential credential attacks early.
