# Linux Server Hardening & Security Audit

**Status: In Development**

A hands-on Linux system administration and security project focused on building a baseline Ubuntu Server environment, applying practical security-hardening measures, and reviewing the system with security audit tooling.

The project will document the configuration before and after hardening so that changes can be explained and evaluated.

## Project Objectives
- Build a dedicated Ubuntu Server virtual machine for testing.
- Review the initial system configuration and security posture.
- Apply sensible SSH and account-security settings.
- Configure host-based firewall rules with UFW.
- Apply system updates and reduce unnecessary exposure.
- Run Lynis security audits and document findings.
- Compare audit results and explain relevant changes.

## Planned Environment and Tools
| Technology | Planned use |
|---|---|
| Ubuntu Server | Linux host under assessment |
| VMware Workstation or another local hypervisor | Isolated virtual lab |
| OpenSSH | Remote administration |
| UFW | Host firewall configuration |
| Lynis | Security auditing |
| Linux shell | System administration and validation |
| Git and GitHub | Version control and documentation |

Exact OS release, VM resources, and tool versions will be recorded when the lab is built.

## Planned Hardening Areas
- [ ] Establish a clean VM baseline
- [ ] Record OS, kernel, users, services, and listening ports
- [ ] Review and harden SSH configuration
- [ ] Apply least-privilege account and sudo practices
- [ ] Configure UFW with a documented allowlist
- [ ] Apply security updates
- [ ] Review enabled services and remove unnecessary exposure
- [ ] Run an initial Lynis audit
- [ ] Apply selected remediation actions
- [ ] Run a follow-up audit
- [ ] Compare findings and document limitations

## Initial Project Structure
```text
Linux-Server-Hardening/
├── README.md
├── docs/
│   ├── project-plan.md
│   ├── hardening-checklist.md
│   └── audit-comparison.md
├── baseline/  # Initial system notes — planned
├── hardening/ # Configuration notes — planned
└── evidence/  # Sanitized audit evidence — planned
```

## Development Roadmap
1. **Lab setup:** create an isolated Ubuntu Server VM and record its baseline.
2. **Initial assessment:** inspect accounts, services, firewall state, and listening ports; run an initial Lynis audit.
3. **Hardening:** implement and document SSH, account, update, and firewall changes.
4. **Validation:** verify that required administrative access remains available and unwanted access is restricted.
5. **Reassessment:** run a second Lynis audit and compare findings.
6. **Reporting:** document changes, evidence, lessons learned, and remaining risks.

## Skills Demonstrated
Linux administration, system hardening, SSH, firewall configuration, least privilege, vulnerability assessment, security auditing, risk analysis, and technical documentation.

## Lab Safety
All configuration changes and tests will be performed on a dedicated virtual machine in an isolated lab. Firewall and SSH changes can interrupt remote access, so a recovery console or snapshot will be maintained before applying them. No production systems will be modified.

---

Planned controls and audit outcomes are not represented as completed until they have been implemented and validated.
