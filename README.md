#  Vulnerability Scan Report – Nessus Essentials

This project documents a basic vulnerability assessment performed on a Windows 11 system using **Tenable Nessus Essentials**. The objective was to identify potential security risks and explore mitigations using common hardening practices.


## 🛠️ Tools Used
- **Nessus Essentials** (Free vulnerability scanner)

     
## ⚠️ Key Vulnerability Identified

### ✅ SMB Signing Not Required
- **Severity:** Medium (CVSS: 5.3)
- **Risk:** Allows unauthenticated, remote attackers to perform man-in-the-middle (MITM) attacks over SMB.
- **Fix:** Enforce SMB signing via Group Policy:
  - `Computer Configuration > Security Settings > Local Policies > Security Options`
  - Enable: `Microsoft network server: Digitally sign communications (always)`


## 🧯 Recommendations

- ✅ **Enable SMB signing**
- 🚫 Disable unused ports (e.g., SMB if not needed)
- 🔄 Regularly update Windows and patch services
- 🔐 Enable Windows Defender Firewall + Network protection
- 🧪 Re-scan monthly to monitor new vulnerabilities


- Scan summary
- Vulnerability details
- Fix recommendation view
