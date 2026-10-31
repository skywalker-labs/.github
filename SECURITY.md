# Security Policy

## Reporting Security Vulnerabilities

At **Skywalker Labs** and the **Skywalker Intelligence System**, security is a foundational architectural layer, not an afterthought. We take the security of our open-source packages, enterprise architectures, and distributed systems seriously.

If you believe you have discovered a vulnerability, security flaw, or potential exposure in any repository or package maintained by **Skywalker Labs**, please report it immediately through our responsible disclosure process.

### Vulnerability Disclosure Channel
- **Email:** [skywalkerlknw@gmail.com](mailto:skywalkerlknw@gmail.com)
- **Subject Line:** `[SECURITY] Potential Vulnerability in <Repository/Package Name>`

> [!IMPORTANT]
> **Please do not report security vulnerabilities through public GitHub issues, discussions, or pull requests.** Always use the private disclosure email above to prevent premature exposure before a patch is prepared and distributed.

---

## Response Timeline & SLAs

When you submit a report, the engineering team commits to the following timeline:
- **Initial Acknowledgment:** Within 48 hours of receipt.
- **Triage & Validation:** Within 5 business days, confirming severity and reproduction steps.
- **Remediation & Patch Release:** Released via semantic patch versions according to CVSS severity ratings.
- **Credit & Advisory:** Public security advisory with credit to the reporter upon patch deployment (unless anonymity is requested).

---

## Supported Versions

We provide security updates and patches for active major release branches of all published packages:

| Major Version | Supported | Security Patches |
| :--- | :---: | :---: |
| Latest Stable (Current) | :white_check_mark: | Active |
| Prior Major (N-1) | :white_check_mark: | Critical CVEs only (6 months post-release) |
| Deprecated (< N-1) | :x: | Unsupported (Upgrade recommended) |

---

## Zero-Trust Security Standard

Skywalker Labs enforces a strict **Zero-Trust Engineering Benchmark**:
- Parameterized SQL binding (SQLi mitigation).
- Mandatory token cryptographic validation & strict session rotation.
- Principle of Least Privilege across RBAC / ABAC access matrices.
- Automated CI/CD dependency vulnerability auditing via Dependabot / static analyzers.

