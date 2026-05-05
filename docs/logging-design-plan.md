# Logging Design Plan

## Status

Planned.

This document will define the planned AWS logging strategy for this lab.

---

## Purpose

The purpose of this document is to identify which AWS log sources are useful for cloud security monitoring and basic investigation.

Logging should support visibility, accountability, alerting, and incident review.

---

## Planned Log Sources

| Log Source | Purpose | Planned Use |
|---|---|---|
| CloudTrail | Records AWS API and account activity | Primary investigation source |
| CloudWatch Logs | Stores and reviews logs from AWS services | Monitoring and review |
| GuardDuty Findings | Identifies suspicious activity | Detection and triage |
| VPC Flow Logs | Captures network flow metadata | Optional / future due to cost |
| S3 Access Logs | Records S3 bucket access | Optional / future |
| EventBridge Events | Routes events for alerting | Alerting workflow |

---

## Logging Goals

The logging design should help answer:

- Who performed an action?
- What action occurred?
- When did it happen?
- Which AWS resource was affected?
- Which source IP was involved?
- Was the action successful or denied?
- Does the activity indicate risk?
- Should an alert be generated?

---

## Detection Use Cases to Explore Later

Potential beginner detection use cases:

| Use Case | Possible Source |
|---|---|
| Root account usage | CloudTrail |
| Failed console login | CloudTrail |
| IAM policy change | CloudTrail |
| Security group modified | CloudTrail |
| S3 public access change | CloudTrail |
| EC2 instance launched | CloudTrail |
| GuardDuty finding generated | GuardDuty / EventBridge |
| Unusual API activity | CloudTrail / GuardDuty |

---

## Logging Workflow

Planned workflow:

1. Generate or identify AWS activity.
2. Review the event in CloudTrail.
3. Identify the actor, action, source, and affected resource.
4. Determine whether the activity is expected.
5. Document investigation notes.
6. Identify whether alerting would be useful.
7. Record lessons learned.

---

## Risks to Consider

| Risk | Why It Matters |
|---|---|
| No logging enabled | Activity cannot be investigated |
| Logs not reviewed | Visibility exists but is not useful |
| Excessive log ingestion | Can create cost |
| Logs stored insecurely | Sensitive event data may be exposed |
| No alerting path | Important events may be missed |
| Poor event documentation | Makes investigations harder |

---

## Planned Evidence

Later implementation may include:

- Logging architecture diagram
- CloudTrail screenshots
- CloudWatch screenshots
- GuardDuty sample finding screenshots
- EventBridge rule screenshots
- Redacted event examples
