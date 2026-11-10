# Linux Server Hardening Checklist

**Status:** Planned checklist — items will be checked only after implementation and verification.

## Baseline
- [ ] Record Ubuntu release and kernel version
- [ ] Record VM resources and network mode
- [ ] Record local users and sudo access
- [ ] Review enabled services
- [ ] Review listening ports
- [ ] Record initial UFW status
- [ ] Run and save initial Lynis audit summary

## SSH
- [ ] Confirm administrative access and recovery console
- [ ] Review SSH configuration and authentication methods
- [ ] Prefer key-based authentication where practical
- [ ] Restrict SSH access to authorized sources where appropriate
- [ ] Validate configuration before restarting SSH
- [ ] Confirm a new session works before closing the recovery session

## Accounts and Updates
- [ ] Review local accounts and remove only confirmed unnecessary accounts
- [ ] Review sudo membership and least privilege
- [ ] Apply available security updates
- [ ] Document update and reboot status

## Firewall and Services
- [ ] Define required inbound services before enabling firewall rules
- [ ] Configure UFW default policies
- [ ] Allow only required inbound ports and trusted sources
- [ ] Enable UFW from the VM console or with a recovery path available
- [ ] Verify required services remain reachable
- [ ] Review and disable unnecessary services only after confirming impact

## Validation and Reassessment
- [ ] Verify administrative access
- [ ] Verify firewall rules and listening ports
- [ ] Run follow-up Lynis audit
- [ ] Compare initial and follow-up findings
- [ ] Document unresolved findings and accepted risks

**Safety reminder:** use a VM snapshot and console access before network, firewall, or SSH changes. Never apply these steps blindly to a production server.
