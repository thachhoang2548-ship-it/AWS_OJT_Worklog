---
title: "Week 8 Worklog"
date: 2026-03-02
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Targets for Week 8

This week marked the shift from planning to execution. We dove into writing the actual code base and weaving foundational AWS services into the application infrastructure.

- **Project Implementation**:
  - Kick off the programming phase for key software features.
  - Forge the linkages connecting frontend clients, backend logic, and the database.
  - Establish a solid technical bedrock for future sprints.

- **Cloud Service Binding**:
  - **Amazon EC2**: Provisioned to host and run backend applications.
  - **Amazon RDS**: Deployed for structured relational data management.
  - **Amazon S3**: Designated for serving static media and handling file uploads.
  - **AWS Map**: Hooked in to provide geographic and mapping functionalities.

- **Quality Assurance & Iteration**:
  - Test and verify data flow across interconnected components.
  - Debug and resolve integration hiccups.
  - Refactor the codebase structure to streamline upcoming features.

---

### Task Breakdown

| Day | Task Description | Started | Completed | Source Link |
| :-: |------------------|:-------:|:---------:|-------------|
|  2  | **Repository Initialization**:<br>- Set up boilerplate<br>- Begin core feature development | 02/03/2026 | 02/03/2026 | Internal |
|  3  | **Backend & DB Hookup**:<br>- Link APIs to RDS<br>- Code rudimentary data queries | 03/03/2026 | 03/03/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  4  | **Asset Storage (S3)**:<br>- Fine-tune S3 buckets<br>- Process static object uploads | 04/03/2026 | 04/03/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  5  | **Geographic Integration**:<br>- Hook up AWS Map<br>- Render coordinates on UI | 05/03/2026 | 05/03/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  6  | **Deployment & Validation**:<br>- Push code to EC2<br>- Conduct end-to-end trials | 06/03/2026 | 06/03/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |

---

### Results of Week 8

#### Milestones Reached

- Initiated the **hands-on coding phase** of the project.
- Successfully bridged the **frontend, backend, and database** ecosystems.
- Attached **Amazon RDS** as the primary persistent storage layer.
- Configured **Amazon S3** effectively for static and media files.
- Successfully embedded **AWS Map** to handle spatial data.
- Ran a successful test deployment directly on **Amazon EC2**.
- Confirmed the operational integrity of the entire end-to-end system sequence.

#### Architecture Key Takeaways

- **Compute Runtime**: Amazon EC2 managing the core application logic.
- **Relational Storage**: Amazon RDS holding systematic business data.
- **Object Storage**: Amazon S3 serving static UI assets and user files.
- **Spatial Services**: AWS Map supplying geographical context.
- **Communication Flow**: Synchronized interactions between Frontend ↔ Backend ↔ AWS infrastructure.
