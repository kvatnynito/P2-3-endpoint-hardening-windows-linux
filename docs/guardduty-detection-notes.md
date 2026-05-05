# GuardDuty Detection Notes

## Status

Planned.

This document will track GuardDuty detection review and finding triage notes.

---

## Purpose

Amazon GuardDuty is an AWS threat detection service that analyzes AWS activity and identifies potentially suspicious behavior.

For this lab, GuardDuty will be reviewed carefully with cost control in mind.

---

## GuardDuty Use in This Portfolio

GuardDuty may be used to:

- Review AWS-native threat detection
- Understand finding severity
- Practice cloud alert triage
- Connect findings to investigation steps
- Document cloud detection workflow

---

## Cost-Control Warning

GuardDuty may have a free trial for new accounts or regions, but it can create charges after the trial period.

Planned controls:

- Confirm trial status before enabling
- Use one region where possible
- Document enablement date
- Review findings during the trial window
- Disable if not actively using after testing
- Monitor billing

---

## Finding Review Questions

When reviewing a GuardDuty finding, answer:

1. What is the finding type?
2. What is the severity?
3. Which resource is affected?
4. Which AWS account or identity is involved?
5. What behavior triggered the finding?
6. What evidence supports the finding?
7. What should be investigated next?
8. What remediation would be appropriate?
9. Is this a true positive, false positive, or test finding?

---

## Planned Finding Fields to Document

| Field | Notes |
|---|---|
| Finding type | To be completed |
| Severity | To be completed |
| Region | To be completed |
| Affected resource | To be completed |
| First seen | To be completed |
| Last seen | To be completed |
| Description | To be completed |
| Investigation notes | To be completed |
| Remediation notes | To be completed |

---

## Example Detection Topics

Potential areas to review:

- Unauthorized access attempts
- Suspicious API behavior
- Reconnaissance activity
- Exposed credentials
- EC2-related suspicious activity
- S3-related suspicious activity

---

## Planned Evidence

Later implementation may include:

- Redacted GuardDuty dashboard screenshot
- Sample finding review
- Triage notes
- Remediation notes
- Lessons learned

---

## Security Notes

GuardDuty findings may contain sensitive details.

Before committing evidence, redact:

- AWS account ID
- ARNs if sensitive
- Public IP addresses if sensitive
- Resource IDs if sensitive
- Usernames if needed
