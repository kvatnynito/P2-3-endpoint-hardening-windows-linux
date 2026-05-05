# P2-3: AWS Logging, Monitoring & Detection

## Overview

This repository is part of **Cybersecurity Portfolio 2: AWS Cloud Security & Engineering**.

The purpose of this project is to design and document AWS-native logging, monitoring, and basic detection workflows. This lab will focus on CloudTrail, CloudWatch, GuardDuty, EventBridge, and cloud investigation concepts.

This project is planned as the third AWS-focused lab in Portfolio 2 because visibility should be established after the account and network foundations are prepared.

---

## Status

**Planned**

This project has not been implemented yet.

Work on this repository will begin after the required Portfolio 1 homelab foundation is completed and after the initial AWS account and VPC foundations are prepared.

Current status:

- [ ] Logging design planned
- [ ] CloudTrail event review planned
- [ ] CloudWatch monitoring plan created
- [ ] GuardDuty review planned
- [ ] EventBridge alerting plan created
- [ ] Cost-control notes created
- [ ] Detection workflow documented
- [ ] Screenshots and evidence collected
- [ ] Final documentation completed

---

## Portfolio Context

### Portfolio 1 Foundation

Portfolio 1 focuses on building a local cybersecurity homelab using Proxmox, pfSense, network segmentation, Active Directory, Splunk, and vulnerable systems.

Portfolio 1 builds the local visibility and monitoring foundation.

### Portfolio 2 Direction

Portfolio 2 expands local infrastructure and security concepts into AWS cloud security and cloud engineering.

This repository focuses on AWS-native logging, monitoring, alerting, and investigation workflows.

---

## Project Goal

The goal of this project is to understand how AWS activity can be logged, monitored, reviewed, and used for basic detection.

By the end of this project, the planned AWS environment should include documentation for:

- AWS CloudTrail logging
- CloudTrail event review
- CloudWatch monitoring basics
- GuardDuty finding review
- EventBridge alerting concepts
- Basic cloud investigation workflow
- Logging cost-control considerations
- Redacted evidence and screenshots

---

## Planned Skills

This project is intended to develop hands-on familiarity with:

- AWS logging concepts
- CloudTrail
- CloudWatch
- GuardDuty
- EventBridge
- Cloud investigation workflow
- API activity review
- Alert triage
- Detection documentation
- Cloud telemetry cost control
- Security monitoring documentation

---

## Planned AWS Services

The following AWS services and features may be used in this project:

| AWS Service / Feature | Planned Use |
|---|---|
| AWS CloudTrail | Record AWS API and account activity |
| Amazon CloudWatch | Monitor logs, metrics, and alarms |
| Amazon GuardDuty | Review threat detection findings |
| Amazon EventBridge | Route events and create basic alerting workflows |
| Amazon S3 | Optional CloudTrail log storage |
| AWS IAM | Generate and review identity-related events |
| Amazon EC2 | Optional test activity source |
| Amazon VPC | Optional network activity context |
| AWS CLI | Optional event generation and validation |

---

## Planned Lab Sections

### 1. Logging Design

Planned tasks:

- Identify required AWS log sources
- Document what each log source records
- Define where logs will be reviewed
- Identify retention and cost concerns
- Create a basic logging workflow diagram

Expected outcome:

> AWS logging sources are documented and connected to security monitoring use cases.

---

### 2. CloudTrail Event Review

Planned tasks:

- Review CloudTrail event history
- Identify common management events
- Review IAM-related activity
- Review console login events
- Review successful and failed API activity
- Document investigation questions

Expected outcome:

> CloudTrail is understood as the primary source for AWS API and account activity investigation.

---

### 3. CloudWatch Monitoring

Planned tasks:

- Review CloudWatch metrics and logs
- Identify basic monitoring use cases
- Document alarm concepts
- Review log group behavior
- Identify cost-control considerations

Expected outcome:

> CloudWatch is understood as a monitoring and observability service for AWS resources and logs.

---

### 4. GuardDuty Detection Review

Planned tasks:

- Enable or review GuardDuty only when cost-controlled
- Review sample findings if available
- Document finding severity
- Document affected resource information
- Practice basic finding triage

Expected outcome:

> GuardDuty findings are reviewed and documented using a basic investigation workflow.

---

### 5. EventBridge Alerting Concepts

Planned tasks:

- Review EventBridge event patterns
- Document how AWS events can trigger actions
- Plan basic alerting workflow
- Connect detection ideas to EventBridge rules
- Avoid unnecessary complexity during initial implementation

Expected outcome:

> EventBridge is understood as a way to route AWS events into alerting or response workflows.

---

## Planned Deliverables

This repository is expected to include:

- Logging design plan
- CloudTrail event review notes
- CloudWatch monitoring plan
- GuardDuty detection notes
- EventBridge alerting plan
- Cost-control notes
- Detection workflow diagram
- Redacted screenshots
- Lessons learned
- Final project summary

---

## Proposed Repository Structure

    P2-3-aws-logging-monitoring-detection/
    ├── README.md
    ├── docs/
    │   ├── logging-design-plan.md
    │   ├── cloudtrail-event-review.md
    │   ├── cloudwatch-monitoring-plan.md
    │   ├── guardduty-detection-notes.md
    │   ├── eventbridge-alerting-plan.md
    │   ├── cost-control-notes.md
    │   └── lessons-learned.md
    ├── diagrams/
    │   └── README.md
    └── screenshots/
        └── README.md

---

## Security Notes

Sensitive information will not be committed to this repository.

This includes:

- AWS account ID
- Access keys
- Secret access keys
- Public IP addresses unless intentionally documented and safe
- Private IP addresses if considered sensitive
- Unredacted ARNs
- Unredacted CloudTrail events containing sensitive details
- Unredacted GuardDuty findings
- Any credential material

Screenshots and event samples will be reviewed and redacted before being uploaded.

---

## Cost-Control Notes

This project is designed to stay within the AWS Free Tier or near-free usage.

Special care will be taken with AWS logging and detection services that can generate cost, especially:

- CloudWatch Logs
- CloudWatch Alarms
- VPC Flow Logs
- GuardDuty after trial period
- S3 log storage
- EventBridge custom events
- High-volume log ingestion

The goal is to learn AWS monitoring and detection without creating unnecessary cost.

---

## Relationship to AWS Solutions Architect Associate

This project supports foundational knowledge for the **AWS Certified Solutions Architect – Associate** certification by focusing on:

- Monitoring
- Logging
- CloudTrail
- CloudWatch
- Security visibility
- Event-driven architecture basics
- Operational excellence
- Cost-aware monitoring design

This repository is not a certification study guide. It is a hands-on portfolio project designed to support practical AWS learning.

---

## Resume Skill Alignment

This project is intended to support resume experience related to:

- AWS logging and monitoring
- CloudTrail event analysis
- CloudWatch monitoring
- GuardDuty finding review
- EventBridge alerting concepts
- Cloud security investigations
- Detection documentation

Example resume bullet after completion:

> Configured and reviewed AWS-native logging and monitoring workflows using CloudTrail, CloudWatch, GuardDuty, and EventBridge to support cloud security visibility and basic incident investigation.

---

## Current Status Summary

This repository is currently in the planning stage.

Implementation will begin after the required Portfolio 1 foundation is completed and after the AWS account and VPC foundations are prepared.
