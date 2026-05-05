# Cost-Control Notes

## Status

Planned.

This document will track cost-control considerations for the AWS Logging, Monitoring & Detection lab.

---

## Purpose

The purpose of this document is to prevent unnecessary AWS costs while testing logging, monitoring, and detection services.

Cloud monitoring tools are useful, but log volume and service trials can create surprise charges if unmanaged.

---

## Services to Watch

| Service / Feature | Cost Risk |
|---|---|
| CloudWatch Logs | Log ingestion and retention may create cost |
| CloudWatch Alarms | Too many alarms can create cost |
| CloudWatch Dashboards | Custom dashboards may create cost |
| Logs Insights | Queries may create cost depending on usage |
| GuardDuty | Can create charges after free trial |
| VPC Flow Logs | Can create log ingestion and storage costs |
| S3 log storage | Storage costs can grow over time |
| EventBridge | Custom event usage may create cost |

---

## Cost-Control Rules

Planned rules:

1. Configure billing alerts before implementation.
2. Use one AWS region where possible.
3. Keep log volume low.
4. Avoid enabling VPC Flow Logs unless needed.
5. Confirm GuardDuty trial status before enabling.
6. Disable GuardDuty if not actively testing after the trial.
7. Review CloudWatch log retention.
8. Delete unused log groups if appropriate.
9. Avoid unnecessary dashboards.
10. Check billing dashboard after lab sessions.

---

## GuardDuty Trial Tracking

If GuardDuty is enabled, track:

| Item | Notes |
|---|---|
| Date enabled | To be completed |
| Region enabled | To be completed |
| Trial end date | To be completed |
| Findings reviewed | To be completed |
| Disable decision | To be completed |

---

## Logging Cleanup Checklist

Before ending each AWS lab session:

- [ ] Review CloudWatch log groups
- [ ] Review log retention settings
- [ ] Review active CloudWatch alarms
- [ ] Review GuardDuty status
- [ ] Review EventBridge rules
- [ ] Review S3 log buckets if used
- [ ] Review VPC Flow Logs if enabled
- [ ] Check billing dashboard
- [ ] Document remaining resources

---

## Evidence to Collect Later

Later implementation may include:

- Redacted billing dashboard screenshot
- GuardDuty trial tracking notes
- CloudWatch log retention notes
- Cleanup notes
- Cost lessons learned
