---
title: "Week 4 Worklog"
date: 2026-01-26
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Targets for Week 4

The theme for this week was architecting structured operations for a production-ready cloud deployment, touching upon automation, defensive security, fault tolerance, system efficiency, and financial control—all aligned with the AWS Well-Architected Framework.

- **Operational Efficiency**:
  - Streamline repetitive chores with AWS Lambda (e.g., auto-stopping EC2 instances, sending Slack alerts).
  - Establish robust telemetry via CloudWatch coupled with Grafana dashboards.
  - Implement structured resource tagging for EC2 instances.
  - Systematize operational management using AWS Systems Manager.

- **Defensive Posture**:
  - Restrict maximum privileges leveraging IAM Permission Boundaries.
  - Conduct thorough compliance checks using AWS Security Hub.
  - Shield web applications from malicious traffic with AWS WAF.

- **Fault Tolerance & Reliability**:
  - Institute comprehensive data protection plans through AWS Backup.
  - Interconnect isolated networks using VPC Peering.
  - Unify network routing utilizing AWS Transit Gateway.

- **System Performance**:
  - Package applications into Docker containers and orchestrate them via ECS.
  - Assemble continuous delivery and integration processes using CodePipeline.
  - Map dynamic file storage dynamically utilizing File Storage Gateway.

- **Financial Control**:
  - Reduce long-term compute expenses by adopting Savings Plans and Reserved Instances.
  - Optimize server capacities via EC2 right-sizing strategies.
  - Track and visually break down AWS billing details.

---

### Task Breakdown

| Day | Task Description | Started | Completed | Source Link |
| :-: |------------------|:-------:|:---------:|-------------|
|  2  | **Ops & Telemetry**:<br>- Lambda automation<br>- CloudWatch & Grafana setup<br>- Implementing Tags<br>- Systems Manager control | 26/01/2026 | 26/01/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  3  | **Cybersecurity**:<br>- IAM Boundaries<br>- Security Hub enablement<br>- WAF configuration | 27/01/2026 | 27/01/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  4  | **Disaster Recovery & Network**:<br>- AWS Backup configurations<br>- Peering VPCs<br>- Transit Gateway setup | 28/01/2026 | 28/01/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  5  | **Efficiency Tuning**:<br>- Dockerization / ECS orchestration<br>- CodePipeline setup<br>- File Storage Gateway binding | 29/01/2026 | 29/01/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  6  | **Billing Optimization**:<br>- Purchasing Savings Plans<br>- Acquiring Reserved Instances<br>- Spending analytics | 30/01/2026 | 30/01/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |

---

### Results of Week 4

#### Milestones Reached

- Engineered automated workflows:
  - Scheduled EC2 shutdowns and integrated Slack notifications via Lambda triggers.
  - Crafted highly visible operational metrics dashboards leveraging CloudWatch and Grafana.
  - Enforced structured grouping of assets through Tags and Systems Manager.

- Bolstered application security:
  - Put strict guardrails in place via **IAM Permission Boundaries**.
  - Activated a sturdy defensive layer with **AWS WAF**.
  - Assessed and continuously monitored compliance via **Security Hub**.

- Guaranteed system stability:
  - Enforced solid disaster recovery capabilities with **AWS Backup**.
  - Facilitated seamless cross-network communications utilizing **VPC Peering** and **Transit Gateway**.

- Maximized processing throughput:
  - Successfully containerized and hosted digital services via **Docker and ECS**.
  - Established a robust foundational CI/CD pipeline.

- Curtailed unnecessary expenditures:
  - Committed to **Savings Plans and Reserved Instances** for steady workloads.
  - Scaled down over-provisioned capacity (**EC2 right-sizing**).
  - Extracted transparent insights from usage metrics to tame cloud spending.

#### Architecture Key Takeaways

- **Operational Engine**: Lambda combined with Systems Manager.
- **Observability Stack**: CloudWatch paired with Grafana.
- **Defense Mechanism**: IAM Permissions Boundary + Web App Firewall (WAF) + Security Hub.
- **Topology Core**: VPC Peering + Transit Gateway Hub.
- **Processing Layer**: Elastic Container Service (ECS) hosting Docker instances.
- **Delivery Pipeline**: AWS CodePipeline.
- **Extended Storage**: File Storage Gateway caching mechanism.
- **FinOps Framework**: Savings Plans + Cost/Usage Tracking.
