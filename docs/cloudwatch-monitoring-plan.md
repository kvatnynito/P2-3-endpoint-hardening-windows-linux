# CloudWatch Monitoring Plan

## Status

Planned.

This document will define the planned CloudWatch monitoring approach for this lab.

---

## Purpose

Amazon CloudWatch provides monitoring and observability for AWS resources and applications.

For this project, CloudWatch will be reviewed as a basic monitoring tool for logs, metrics, and alarms.

---

## Planned CloudWatch Areas

| Area | Planned Use |
|---|---|
| Metrics | Review basic AWS service metrics |
| Log Groups | Review stored logs |
| Alarms | Create or document basic alert concepts |
| Dashboards | Optional / future |
| Log Insights | Optional / future |
| Billing alarms | Related cost-control use case |

---

## Monitoring Goals

CloudWatch monitoring should help answer:

- Is a resource active?
- Is resource usage abnormal?
- Are logs being collected?
- Has a threshold been crossed?
- Should an alarm notify someone?
- Is monitoring cost under control?

---

## Possible Monitoring Use Cases

| Use Case | CloudWatch Feature |
|---|---|
| EC2 CPU usage | Metrics / Alarm |
| Billing threshold | Alarm |
| Log review | Log Groups |
| CloudTrail log review | Log Groups, if integrated |
| Failed activity search | Logs Insights, if used |
| GuardDuty alert workflow | EventBridge / CloudWatch integration |

---

## Alarm Planning

Potential alarms to document later:

| Alarm | Purpose |
|---|---|
| Billing threshold alarm | Detect unexpected charges |
| EC2 CPU alarm | Basic resource monitoring |
| Log metric alarm | Detect specific log pattern |
| GuardDuty finding event | Alert on security finding |

---

## Cost Considerations

CloudWatch can create cost through:

- Log ingestion
- Log retention
- Metrics
- Alarms
- Dashboards
- Logs Insights queries

Planned controls:

- Keep log volume low
- Avoid unnecessary dashboards
- Use short test periods
- Review log retention
- Delete unused log groups after testing if appropriate

---

## Planned Evidence

Later implementation may include:

- CloudWatch metrics screenshot
- Log group screenshot
- Alarm configuration screenshot
- Notes about monitoring limitations
- Lessons learned
