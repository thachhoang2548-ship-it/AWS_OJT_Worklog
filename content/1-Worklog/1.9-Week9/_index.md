---
title: "Week 9 Worklog"
date: 2026-03-09
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Targets for Week 9

This week centered around trial deployments, holistic system testing, and remediating bugs identified during the initial staging phase.

- **Infrastructure Deployment**:
  - Spin up the application in a staging environment on Amazon EC2.
  - Bind the application to auxiliary services like RDS, S3, and AWS Map.
  - Validate network communication across all architectural tiers.

- **Quality Assurance Testing**:
  - Execute test cases for core business workflows.
  - Scrutinize the user interface and overall experience.
  - Trace data exchanges between the client and server.

- **Troubleshooting and Refactoring**:
  - Patch defects discovered during QA cycles.
  - Refactor code segments to boost system resilience.
  - Implement necessary performance tweaks.

- **Pre-launch Verification**:
  - Guarantee the application's operational stability.
  - Setup the environment for formal demonstration or soft release.

---

### Task Breakdown

| Day | Task Description | Started | Completed | Source Link |
| :-: |------------------|:-------:|:---------:|-------------|
|  2  | **Staging Deployment**:<br>- EC2 hosting configuration<br>- Environment variables setup | 09/03/2026 | 09/03/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  3  | **E2E Testing**:<br>- Feature verification<br>- Data pipeline checks | 10/03/2026 | 10/03/2026 | Internal |
|  4  | **Defect Resolution**:<br>- Log analysis<br>- Bug fixing | 11/03/2026 | 11/03/2026 | Internal |
|  5  | **Code Optimization**:<br>- Architectural refactoring<br>- Speed enhancements | 12/03/2026 | 12/03/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  6  | **Demo Prep**:<br>- Final system check<br>- Demo scenario planning | 13/03/2026 | 13/03/2026 | Internal |

---

### Results of Week 9

#### Milestones Reached

- Seamlessly migrated the application code to **Amazon EC2**.
- Confirmed solid integrations with crucial AWS resources:
  - **Amazon RDS**
  - **Amazon S3**
  - **AWS Map**
- Conducted exhaustive end-to-end testing across primary user journeys.
- Successfully resolved all critical bugs flagged during the QA phase.
- Elevated system performance and smoothed out UX friction points.
- Achieved a stable, **demo-ready** application state.

#### Architecture Key Takeaways

- **Compute Runtime**: EC2 (hosting environment).
- **Persistent Data**: RDS running SQL Server.
- **Static Asset Storage**: S3.
- **Mapping Utilities**: AWS Map.
- **Data Pipeline**: Client UI → Server Logic → AWS Managed Services.
- **Current Phase**: Quality Assurance / Staging Deployment.
