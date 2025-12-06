---
title: "Event 5"
date: "2025-11-29"
weight: 5
chapter: false
pre: " <b> 4.5. </b> "
---

# Summary Report: “AWS Well-Architected Security Pillar”

### Event Objectives

- **Identity & Access Management (IAM)**: Explore modern IAM architecture, emphasizing the importance of avoiding long-term credentials and leveraging AWS Identity Center for short-term credentials.
- **Detection & Continuous Monitoring**: Highlight the significance of multi-layer security visibility and automated detection mechanisms.
- **Infrastructure Protection**: Discuss network and workload security strategies, including segmentation and workload protection.
- **Data Protection**: Understand encryption practices, key management, and secrets rotation.
- **Incident Response**: Learn about the IR lifecycle and automation techniques for effective incident handling.

### Key Highlights

#### Pillar 1 — Identity & Access Management
- **Modern IAM Architecture**: Presented by Huynh Hoang Long and Aiden, this session covered IAM users, roles, and policies, emphasizing the avoidance of long-term credentials. AWS Identity Center was introduced for SSO and permission sets.
- **SCP & Permission Boundaries**: Explained the role of Service Control Policies (SCPs) in managing multi-account environments. SCPs filter permissions but do not grant them.
- **MFA & Credential Rotation**: Compared TOTP and FIDO2 for multi-factor authentication. Recommendations included avoiding IAM users with long-term keys and using AWS Identity Center for short-term credentials.
- **Access Analyzer**: Demonstrated how to validate IAM policies and simulate access permissions.
- **Mini Demo**: Validated IAM policies and simulated access scenarios.

#### Pillar 2 — Detection
- **Detection & Continuous Monitoring**: Presented by Tran Duc Anh, Nguyen Tuan Thinh, and Nguyen Do Thanh Dat, this session emphasized multi-layer security visibility, including management events, data events, and network activity events.
- **CloudTrail & GuardDuty**: Discussed organization-level logging with CloudTrail and the use of GuardDuty for threat detection. Detection-as-code practices were demonstrated, including CloudTrail Lake queries and automated deployments.
- **Advanced Protection Plan**: Covered GuardDuty’s extended threat protection features, including S3 protection, EKS protection, and malware detection.
- **Security Hub**: Highlighted centralized alerting and normalization using AWS Security Hub, which simplifies data analysis and filtering.
- **Alerting & Automation**: Highlighted the use of EventBridge for alerting and automation, along with logging at all layers (e.g., VPC Flow Logs, ALB/S3 logs).

#### Pillar 3 — Infrastructure Protection
- **Network & Workload Security**: Covered VPC segmentation, private vs. public placement, and the application of Security Groups vs. NACLs. Additional topics included WAF, Shield, and Network Firewall for enhanced protection.
- **Common Network Attack Vectors**: Discussed outbound, east-west, and inbound attack scenarios, along with protection use cases.
- **Layered Security**: Introduced AWS layered security approaches, including Route53 VPC DNS resolver and DNS Firewall features.
- **Workload Protection**: Discussed security basics for EC2, ECS, and EKS workloads.

#### Pillar 4 — Data Protection
- **Encryption & Key Management**: Explored KMS key policies, grants, and rotation. Encryption practices for data at rest and in transit were demonstrated for S3, EBS, RDS, and DynamoDB.
- **Secrets Management**: Discussed patterns for secrets rotation using Secrets Manager and Parameter Store. Data classification and access guardrails were also highlighted.

#### Pillar 5 — Incident Response
- **IR Playbook & Automation**: Presented the IR lifecycle according to AWS. Playbooks for common scenarios, such as compromised IAM keys, S3 public exposure, and EC2 malware detection, were shared. Automation techniques using Lambda and Step Functions were demonstrated for auto-response.
- **Prevention Strategies**: Emphasized the importance of eliminating long-lived credentials, avoiding direct S3 bucket exposure, and enforcing infrastructure-as-code (IaC) to prevent misconfigurations.
- **Incident Response Process**: Detailed the five-step process:
  1. **Preparation**: Develop playbooks, train teams, and implement proper tooling.
  2. **Detection and Analysis**: Use GuardDuty findings, CloudTrail anomalies, and Security Hub alerts.
  3. **Containment**: Isolate resources, revoke credentials, and preserve evidence.
  4. **Eradication and Recovery**: Remove threats, patch vulnerabilities, and restore from clean backups.
  5. **Post-Incident Review**: Learn lessons, update playbooks, and improve detection mechanisms.

### Event Experience

The event was highly engaging, with a well-structured agenda that allowed participants to gain in-depth knowledge of AWS security practices. The speakers effectively communicated complex concepts, making them accessible to attendees with varying levels of expertise. The live demonstrations and real-world case studies provided practical insights, enhancing the overall learning experience.

### Lessons Learned

1. **Proactive Security Measures**: The importance of adopting a proactive approach to cloud security, including the use of automation and continuous monitoring, was a key takeaway.
2. **Shared Responsibility Model**: Understanding the shared responsibility model is critical for ensuring security in cloud environments.
3. **Incident Preparedness**: Developing and maintaining incident response playbooks and automating responses can significantly reduce the impact of security incidents.
4. **Continuous Improvement**: Regularly updating security practices and tools is essential to address evolving threats.

### Key Takeaways

- **Identity & Access Management**: Avoid long-term credentials and leverage AWS Identity Center for enhanced security.
- **Detection & Monitoring**: Implement multi-layer security visibility using tools like CloudTrail, GuardDuty, and Security Hub.
- **Infrastructure Protection**: Utilize advanced protection tools such as WAF, Shield, and Network Firewall to secure workloads.
- **Data Protection**: Encrypt data at rest and in transit, and manage secrets securely with AWS KMS and Secrets Manager.
- **Incident Response**: Automate incident response processes and ensure teams are well-prepared with updated playbooks and training.

### Some event photos

![pic1](/images/event5_1.jpg)
![pic2](/images/event5_2.jpg)
![pic3](/images/event5_3.jpg)

> Overall, the event provided a comprehensive overview of the AWS Well-Architected Security Pillar, emphasizing best practices and automation techniques to enhance security posture. Participants gained valuable insights into securing cloud environments effectively. The sessions highlighted the importance of proactive measures, continuous monitoring, and leveraging AWS tools to build resilient and secure infrastructures.