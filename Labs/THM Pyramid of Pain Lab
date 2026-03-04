1. Objective

Investigate indicators of compromise (IOCs) generated from a malware sample using threat intelligence and network analysis tools.

2. Tools Used

List the tools from the lab:

• TryHackMe
• Any.run
• VirusTotal
• Tshark / Wireshark
• Threat Intelligence Sources

3. Indicators Identified

Example indicators from the lab:

Malicious Domains
craftingalegacy.com
Suspicious IP
96.126.101.6

Malicious Executables
Stealer.exe
payload.exe
Ben14fG_juqk.exe

4. Host Artifacts Observed

Suspicious process chain:

WINWORD.exe → PowerShell.exe

This behavior indicates a macro-based malware execution.

Files dropped in:

AppData\Local\Temp

Common attacker tactic for malware persistence.

5. Network Activity

Observed HTTP POST requests communicating with external infrastructure.

Example:

POST request to 96.126.101.6:8080

This indicates Command & Control (C2) communication.

6. Malware Analysis

Hashes were analyzed using threat intelligence platforms.

Example techniques used:

• SHA256 hash lookup
• SSDeep fuzzy hashing
• malware sample comparison

7. Detection Strategy

Defenders could detect this attack using:

• SIEM alerts for Word spawning PowerShell
• IDS detection of unusual POST requests
• threat intelligence blocking malicious domains
• YARA rules for malware signatures

8. Key Lessons

• Malware often uses Office macros to execute PowerShell
• Network traffic analysis reveals C2 communication
• Host artifacts help identify malware persistence
• TTP analysis is the most effective detection level
