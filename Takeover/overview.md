The Takeover room on TryHackMe explores a common web security issue known as subdomain takeover. This vulnerability arises when a DNS record points to an external or cloud resource that no longer exists — for example, a deleted AWS S3 bucket or a misconfigured cloud service. An attacker can claim the orphaned resource and serve malicious content under the legitimate domain.
🔍 Tools & Techniques Used
During this room, the following tools and approaches were applied:
Browser & Certificate Inspection
Used to examine TLS certificates and discover additional subdomains through Subject Alternate Name (SAN) fields.
Hosts File Modification
Mapped discovered subdomains to the target IP for local resolution and testing.
HTTP Interaction Analysis
Observed how the server and browser responded to specific subdomain requests.
Cloud Service Identification
Confirmed how a misconfigured DNS entry pointed to an unused AWS S3 bucket (common web host).
Web Reconnaissance Techniques
Applied logical reasoning and DNS understanding to trace the root cause of the exposure.
🧠 Skills Practiced
DNS Analysis:
Understood how DNS records can outlive associated cloud resources and introduce security gaps.
Subdomain Enumeration:
Identified valid and hidden subdomains using certificate data and manual exploration.
Misconfiguration Identification:
Recognized when DNS points to a nonexistent service — the hallmark of a subdomain takeover risk.
Web Response Interpretation:
Distinguished between valid content responses and error/bucket hosting pages.
🧩 Key Concepts Covered
Operational Vulnerability:
Subdomain takeover is not a traditional code exploit — it's a configuration flaw rooted in DNS and cloud lifecycle management.
Cloud Dependency Awareness:
Modern applications often rely on cloud services (S3, GitHub Pages, etc.). Misalignment between DNS and service resources causes security issues.
Proactive Asset Management:
Regular inventory and cleanup of DNS entries and cloud assets is essential to maintain a secure environment.
💡 Real‑World Relevance
Subdomain takeover vulnerabilities are often exploited in phishing campaigns, content spoofing, and brand hijacking. Attackers use misconfigured subdomains to:
Host deceptive login forms
Distribute malicious content
Bypass user trust due to legitimate domain names
Understanding this risk helps in securing enterprise networks, cloud deployments, and externally visible applications.
🧠 Takeaway
Effective web security assessment requires not only finding code bugs, but also identifying operational and configuration vulnerabilities. Subdomain takeover showcases how infrastructure and DNS weaknesses can be as impactful as software flaws.
