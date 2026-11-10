# Project Plan — Linux Server Hardening & Security Audit

**Status:** In Development

## Purpose
Create a repeatable Linux security-hardening exercise that demonstrates how to establish a baseline, apply selected defensive controls, and assess the resulting configuration.

## Scope
The initial target is a dedicated Ubuntu Server virtual machine. The work will focus on host configuration and security review, not exploitation or production deployment.

## Planned Workflow
1. Create and snapshot a clean Ubuntu Server VM.
2. Record release information, users, enabled services, listening ports, and firewall state.
3. Run an initial Lynis audit and save sanitized output.
4. Review findings and prioritize practical remediation.
5. Apply documented SSH, account, update, and firewall changes.
6. Validate remote administration and required services.
7. Run a second audit and compare findings.
8. Summarize improvements, unresolved findings, and limitations.

## Planned Deliverables
- [ ] Lab build and baseline notes
- [ ] Initial audit summary
- [ ] SSH hardening notes
- [ ] Account and privilege review
- [ ] UFW firewall policy
- [ ] Update and service review
- [ ] Validation checklist
- [ ] Before-and-after audit comparison
- [ ] Final project summary

## Documentation Standards
Record the exact commands and configuration changes used. Redact IP addresses, hostnames, usernames, and other details that should not be public. A change is complete only after it is validated.
