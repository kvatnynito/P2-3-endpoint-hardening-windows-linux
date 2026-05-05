# CloudTrail Event Review

## Status

Planned.

This document will track CloudTrail event review and investigation notes.

---

## Purpose

AWS CloudTrail records AWS API activity and account actions. This document will be used to review CloudTrail events and understand how AWS activity appears during an investigation.

---

## CloudTrail Investigation Questions

When reviewing an event, answer:

1. What event occurred?
2. What AWS service was involved?
3. Which identity performed the action?
4. When did the event happen?
5. What source IP was used?
6. What resource was affected?
7. Was the action successful or denied?
8. Was the activity expected?
9. What risk could this event represent?
10. Should this activity generate an alert?

---

## Planned Events to Review

| Event Type | Why It Matters |
|---|---|
| Console login | Shows interactive account access |
| Failed login | May indicate access issues or attack attempts |
| IAM user creation | Identity changes are high-value security events |
| IAM policy attachment | Permission changes can increase risk |
| Security group change | Network exposure may change |
| S3 bucket policy change | Data exposure risk |
| EC2 instance launch | New compute resource created |
| CloudTrail configuration change | Logging tampering risk |

---

## Event Review Template

| Field | Notes |
|---|---|
| Event name | To be completed |
| Event source | To be completed |
| AWS region | To be completed |
| Event time | To be completed |
| User identity | To be completed |
| Source IP address | To be completed |
| User agent | To be completed |
| Resource affected | To be completed |
| Error code | To be completed |
| Expected or suspicious | To be completed |
| Investigation notes | To be completed |

---

## Example Findings to Document Later

Possible review examples:

- Normal administrator login
- Failed login attempt
- IAM policy change
- Security group modified
- S3 bucket setting changed
- CloudTrail lookup event

---

## Security Notes

CloudTrail events can include sensitive data.

Before committing evidence, redact:

- AWS account ID
- ARNs if sensitive
- Usernames if needed
- Public IP addresses if sensitive
- Resource names if sensitive
- Request parameters if sensitive

---

## Lessons Learned

To be completed after implementation.
