# local-host-vulnarebality-scan
i have done a vulnerability scan on ip and this is my report on it
uefhyfgefkefgylafervte7iete
uefhyfgefkefgylafervte7iete
Update README.md
cb3edf0
🔍 Overall Vulnerability Summary
Severity	Count
🔴 Critical	0
🔶 High	0
🟠 Medium	2
🔵 Low	0
⚪ Info	34
⚠️ Top Vulnerabilities Found
1. SSL Certificate Cannot Be Trusted
Plugin ID: 51192
Severity: Medium
CVSS v3 Score: 6.5
Description:
The SSL certificate installed on this host cannot be trusted. This may be due to a self-signed certificate, expired certificate, or one issued by an untrusted authority.
Impact:
Attackers could perform Man-in-the-Middle (MITM) attacks if users connect to this system assuming the connection is secure.
Fix / Mitigation:
Replace self-signed or expired certificates with valid SSL certificates from a trusted Certificate Authority (CA).
Regularly renew certificates before expiry.
Ensure the server uses modern TLS protocols (1.2 or 1.3) only.
2. SMB Signing Not Required
Plugin ID: 57608
Severity: Medium
CVSS v3 Score: 5.3
Description:
SMB (Server Message Block) signing is not required on the system. This allows attackers to perform relay or impersonation attacks within a local network.
Impact:
Could allow attackers to modify or intercept SMB traffic between clients and servers.
Fix / Mitigation:
Enable SMB signing via Group Policy:
Navigate to:
Computer Configuration > Windows Settings > Security Settings > Local Policies > Security Options
Enable:
“Microsoft network server: Digitally sign communications (always)”
“Microsoft network client: Digitally sign communications (always)”
Reboot the system for changes to take effect.
ℹ️ Informational Findings
Additional DNS Hostnames Detected (Plugin ID: 46180)
Indicates multiple DNS hostnames point to the same IP.
Not a threat, but useful for asset inventory.
🧰 Next Steps
Apply the SSL certificate fix first, as it affects secure communication.
Configure SMB signing to strengthen internal network defense.
Re-scan the system to verify the fixes.
Keep your OS and applications updated and patched regularly.
Prepared by: patnala nikhitha sai Internship Task: Basic Vulnerability Scan
Date: 2025-10-25

About
i have done a vulnerability scan on ip and this is my report on it

Resources
 Readme
 Activity
Stars
 0 stars
Watchers
 0 watching
Forks
 0 forks
Report repository
Releases
No releases published
Packages
No packages published
Languages
HTML
100.0%
Footer
