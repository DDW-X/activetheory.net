# Security Policy

## 1. Supported Versions & Scope

This repository is an independent academic research project, systems architecture dissection, and reverse-engineering case study focusing on the Active Theory production client-side engine.

| Component / Subsystem | Supported for Security Reports | Scope |
| :--- | :---: | :--- |
| Telemetry & Profiling Scripts | :white_check_mark: | Headless CDP harnesses & Node.js test scripts |
| Architectural Documentation | :white_check_mark: | Mathematical formulas & citations |
| Upstream Active Theory Services | :x: | Cloud endpoints / production servers (Report directly to Active Theory LLC) |

---

## 2. Vulnerability Reporting Protocol

We prioritize the security, integrity, and safety of researchers, developers, and upstream platform owners. If you discover a security vulnerability, credential leakage, or potential exploit within this research repository, please follow our responsible disclosure protocol:

### Reporting Channel
- **Email**: Send detailed vulnerability reports directly to:  
  **`ml3740965@gmail.com`**
- **Subject Prefix**: `[SECURITY VULNERABILITY] - <Subsystem / File Name>`

### Required Information
To help us triage and remediate the issue efficiently, please include:
1. **Description**: Clear description of the vulnerability, its potential impact, and classification (e.g., Remote Code Execution, Information Disclosure, Prototype Pollution).
2. **Steps to Reproduce**: Minimal, deterministic proof-of-concept (PoC) code or CLI commands.
3. **Affected Files / Offsets**: Specific file paths or line ranges within this repository.
4. **Remediation Suggestions**: Recommended patches or defensive mitigations, if known.

---

## 3. Response & Remediation Timelines

- **Initial Acknowledgment**: Within **24 hours** of report receipt.
- **Triage & Validation**: Within **48 to 72 hours**.
- **Remediation & Patching**: Within **7 business days** (or sooner for high/critical severity).
- **Public Disclosure**: Coordinated disclosure strictly after a patch has been validated and merged.

---

## 4. Academic Fair Use & Compliance Concerns

If you are an authorized representative or copyright holder representing **Active Theory LLC** or an affiliated commercial client, and you have compliance, intellectual property, or takedown inquiries, please review [README.md Section 7.4](README.md#74-takedown-notices--rights-holder-protocol) and contact `ml3740965@gmail.com` with the subject prefix `[Compliance / IP Notice]`. Verified requests will be addressed with priority remediation within **24 to 48 hours**.
