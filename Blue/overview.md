The Blue room on TryHackMe focuses on exploiting a critical Windows SMB vulnerability (MS17‑010 / EternalBlue).
This lab demonstrates how outdated systems can be fully compromised due to unpatched services — a vulnerability widely abused by real-world ransomware like WannaCry and NotPetya.
🛠 Skills & Techniques Practiced
Network Enumeration
Identified exposed SMB services on a Windows machine
Assessed service versions and security posture
Vulnerability Identification
Confirmed presence of MS17‑010 (EternalBlue)
Understood why SMBv1 is dangerous and deprecated
Exploitation with Metasploit
Used a controlled exploit to gain remote code execution
Achieved system-level access on the target
Post‑Exploitation Awareness
Validated access and impact
Understood privilege context and attacker capabilities
🔍 Key Learning Points
Unpatched systems = full compromise
SMB vulnerabilities can allow unauthenticated remote exploitation
One exposed service can lead to complete system takeover
Patch management is a critical security control, not optional
💡 Real‑World Relevance
This exact vulnerability has been used in:
Ransomware outbreaks
Wormable malware campaigns
Large-scale enterprise breaches
Successfully completing this lab shows the ability to:
Identify high‑risk vulnerabilities
Validate exploitability (not just scan results)
Understand attacker impact on Windows environments
🧠 Security Takeaway
EternalBlue is a reminder that legacy systems and poor patching can destroy entire networks.
A single vulnerable service can compromise confidentiality, integrity, and availability.
👨‍💻 Professional Context
As a Penetration Tester, this lab reflects skills in:
Vulnerability validation
Exploit-based risk assessment
Translating technical findings into real security impact
This experience is directly relevant to:
Penetration Testing
Red Teaming
Vulnerability Assessment
Security Consulting
