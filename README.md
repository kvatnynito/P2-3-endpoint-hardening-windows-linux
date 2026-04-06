# P2-3: Endpoint Hardening (Windows & Linux)

## Overview

This repo is planned to document practical endpoint hardening across both Windows and Linux systems.

It is intended to focus on security baselines, configuration changes, validation steps, and before-and-after evidence showing how systems in the Proxmox-based lab environment are strengthened against common attack paths and misconfigurations.

This project is part of Portfolio 2 and is planned as a follow-on phase after completion of Portfolio 1, which provides the segmented lab foundation used for system deployment, testing, and validation.

---

## Status

**Current state:** Planned  
**Execution state:** Not yet started  
**Prerequisite:** Portfolio 1 completion

This repo is being prepared in advance so that the project scope, target systems, validation approach, and expected deliverables are already defined before hands-on hardening begins.

---

## Planned Objectives

This project is intended to build practical endpoint hardening skills, including:

- creating Windows and Linux hardening baselines
- applying secure configuration changes
- validating results with system and security tools
- capturing before-and-after evidence
- reducing exposure to common attacker techniques and avoidable misconfigurations

---

## Planned Repository Structure

- `docs/` — baselines, checklists, templates, hardening notes, and validation guidance
- `lab/` — validation outputs, screenshots, and before-and-after comparisons
- `scripts/` — optional auditing, validation, or configuration support scripts
- `.github/` — issue or pull request templates (optional)

---

## Planned Lab Setup

### Host Platform
This project is planned to use the Proxmox-based lab environment built in Portfolio 1.

### Planned Operating Systems

#### Windows Targets
Planned Windows systems may include:

- Windows 10
- Windows 11
- Windows Server 2019

#### Linux Targets
Planned Linux systems may include:

- Ubuntu 22.04
- Debian
- other Linux systems already deployed in the lab as needed

### Planned Network Design
- pfSense-based segmentation carried forward from Portfolio 1
- systems placed in the appropriate lab segment based on role and trust level
- optional use of Active Directory later for GPO-based Windows hardening where relevant

---

## Planned Tools

### Windows
Planned tools and validation sources may include:

- Sysinternals Suite
- PowerShell
- Microsoft Security Baselines
- Local Group Policy Editor (`gpedit.msc`)
- `secedit`
- `gpresult`

### Linux
Planned tools and validation sources may include:

- Lynis
- auditd
- UFW
- `iptables` where applicable
- `sysctl`

Some validation steps may later be compared against logging or telemetry collected through the broader lab environment when relevant.

---

## Planned Hardening Focus Areas

### Windows
Planned Windows hardening areas may include:

- local security policies
- RDP restrictions
- PowerShell logging
- firewall configuration
- SMB security settings
- secure user rights assignments
- attack surface reduction where supported
- removal or disablement of unnecessary roles, features, or services

### Linux
Planned Linux hardening areas may include:

- SSH hardening
- password and account lockout policies
- file permissions
- firewall configuration
- auditd rule validation
- disabling unused services
- kernel parameter hardening with `sysctl`
- log retention and basic audit visibility

---

## Planned Validation Workflow

Once execution begins, the intended workflow for this repo is:

### 1. Establish a baseline
Planned activities may include:

- documenting the initial system state
- recording relevant default or existing settings
- capturing screenshots or exports before changes are applied

### 2. Apply hardening changes
Planned activities may include:

- adjusting local security settings
- disabling or restricting risky services
- applying firewall and logging improvements
- enabling additional protections where supported by the operating system

### 3. Validate the results
Planned activities may include running validation commands and collecting output.

#### Windows Validation
Example commands may include:

```powershell
Get-ProcessMitigation
Get-MpComputerStatus
secedit /export /cfg baseline.cfg
gpresult /h report.html
```

Planned evidence may include:

- before-and-after screenshots
- policy reports
- mitigation status results
- exported configuration output

#### Linux Validation
Example commands may include:

```bash
sudo lynis audit system
sudo ufw status
cat /etc/ssh/sshd_config
sudo sysctl -a
```

Planned evidence may include:

- Lynis audit results
- SSH configuration changes
- kernel hardening output
- firewall status and rules
- screenshots or saved command output

### 4. Compare before and after state
Planned activities may include:

- documenting what changed
- identifying security improvements made
- noting any tradeoffs or functionality considerations
- saving repeatable evidence in the repo

---

## Planned Deliverables

This repo is expected to eventually include:

- Windows hardening baseline documentation
- Linux hardening baseline documentation
- before-and-after screenshots
- validation reports and command output
- optional architecture or configuration diagrams
- helper scripts for auditing or validation
- notes explaining security improvements made to each system

---

## Planned Skill Areas

This project is intended to help build experience in:

- secure baseline development
- Windows and Linux system hardening
- validation of security settings
- understanding how weak configurations are abused
- reducing attack surface without breaking core functionality
- documenting system changes clearly and professionally
- applying the principle of least privilege in practical ways

---

## Planned Next Steps

When work begins on this repo, the initial implementation focus will likely be:

- select the first Windows and Linux targets in the Proxmox lab
- document baseline system state before changes
- apply initial hardening steps
- validate results with native tools and audit utilities
- store before-and-after evidence in a repeatable format

Future expansion may include:

- Active Directory and GPO-based Windows hardening
- Microsoft official security baseline comparisons
- CIS benchmark comparisons
- automated validation checks using PowerShell or Bash
- scripts to export or compare baseline configurations
- additional operating system coverage later if useful

---

## License

MIT — see `LICENSE`.
