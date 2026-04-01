---
title: "Week 2 Worklog"
date: 2026-01-12
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Targets for Week 2

The core theme of this week was establishing secure access controls and designing a robust AWS network architecture. We moved from standard configurations to more complex setups. The main goals were:

- **Identity and Access Management (IAM)**:
  - Generate new Users and Groups.
  - Apply the correct permission Policies.
  - Define and utilize IAM Roles.
  - Gain hands-on experience with **Switch Role**.

- **Mastering VPC Fundamentals**:
  - Grasp the overall VPC structure.
  - Differentiate between **NACLs and Security Groups**.
  - Lay the networking groundwork to host EC2 instances.

- **EC2 Deployment**:
  - Provision EC2 instances within designated subnets.
  - Set up necessary Security Group firewall rules.
  - Establish remote SSH access using Key Pairs.

- **Hybrid DNS Integration with Route 53 Resolver**:
  - Generate a secure Key Pair.
  - Adjust Security Group settings.
  - DNS Configuration steps:
    - Launch an Outbound Endpoint.
    - Define Resolver routing rules.
    - Deploy an Inbound Endpoint.
  - Remove unnecessary resources afterward.

- **Configuring VPC Peering**:
  - Understand the concept of VPC Peering.
  - Provision the base infrastructure using CloudFormation.
  - Boot up EC2 instances and attach Security Groups.
  - Modify Network ACL rules.
  - Complete the Peering Connection setup.
  - Route Tables adjustment.
  - Turn on DNS resolution across peers.

- **Implementing AWS Transit Gateway**:
  - Provision a Transit Gateway.
  - Attach the participating VPCs.
  - Set up routing rules within the Transit Gateway.
  - Modify individual VPC Route Tables accordingly.

---

### Task Breakdown

| Day | Task Description | Started | Completed | Source Link |
| :-: |------------------|:-------:|:---------:|-------------|
|  2  | **Core IAM & EC2**:<br>- User/Group mapping<br>- Policy assignment<br>- Role switching<br>- EC2 provisioning & SSH | 12/01/2026 | 12/01/2026 | [AWS Study Group](https://www.facebook.com/groups/awsstudygroupfcj/) |
|  3  | **VPC Infrastructure**:<br>- VPC concepts<br>- SG vs NACL comparison<br>- Subnet layout preparation | 13/01/2026 | 13/01/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  4  | **Route 53 Hybrid DNS**:<br>- Key Pair setup<br>- SG rules<br>- Inbound/Outbound Endpoints<br>- Resolver configuration | 14/01/2026 | 14/01/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  5  | **VPC Peering Setup**:<br>- CloudFormation deployment<br>- EC2/SG configuration<br>- Link peering connection<br>- Route adjustments<br>- DNS enablement | 15/01/2026 | 15/01/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  6  | **Transit Gateway (TGW)**:<br>- Setup TGW<br>- VPC attachments<br>- Routing setup | 16/01/2026 | 16/01/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |

---

### Results of Week 2

#### Milestones Reached

- Acquired deep practical knowledge of **IAM** and the **Switch Role** functionality.
- Gained proficiency in **VPC network topology** and network-level defense layers.
- Confidently spun up an **EC2 instance** and accessed it via SSH.
- Set up a functional **Hybrid DNS** architecture using Route 53 Resolvers.
- Bridge Dev and Staging networks successfully via **VPC Peering**.
- Centralized network routing using **AWS Transit Gateway**.
- Introduced **Infrastructure as Code (IaC)** principles with AWS CloudFormation.
- Faithfully executed **resource cleanup** to optimize costs.

#### Architecture Key Takeaways

- **IAM Hierarchy**: Users → Groups → Policies → Roles (enables dynamic permissions).
- **VPC Defense Approach**:
  - Security Groups: Stateful instance-level control.
  - NACLs: Stateless subnet-level boundary control.
- **Hybrid DNS Flow**:
  - Route 53 Resolver Endpoints bridging On-premises and AWS environments.
- **Network Topologies**:
  - VPC Peering: Direct 1-to-1 network link.
  - Transit Gateway: Scalable hub-and-spoke centralized design.
