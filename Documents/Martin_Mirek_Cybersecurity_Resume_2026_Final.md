# MARTIN MIREK

**Cloud Security • Identity & Access Management • Security Operations**

Oakville, ON | (289) 696-7208 | [Martin.Mirek@gmail.com](mailto:Martin.Mirek@gmail.com) | [LinkedIn](http://www.linkedin.com/in/martin-mirek91) | [GitHub](https://github.com/Marteus5?tab=repositories)

---

## Professional Summary

Cybersecurity diploma student (Sheridan College) with 5+ years of technical support experience in fintech and telecommunications, including payment systems troubleshooting at Moneris. Hands-on with AWS cloud security: built Terraform-provisioned network segmentation and demonstrated, exploited, and remediated a real AWS IAM privilege escalation path. Pursuing AWS certifications. Seeking an entry-level Cloud Security Analyst role, with strong interest in Identity & Access Management and SOC Analyst positions, in a financial services environment.

## Technical Skills

| Area | Skills |
|:-----|:-------|
| **Cloud Security** | AWS (VPC, subnetting, NACLs, Security Groups, EC2, S3), network segmentation, bastion / jump host design, Infrastructure as Code (Terraform) |
| **Identity & Access** | AWS IAM policies, least privilege, privilege escalation analysis & remediation, access reviews, cryptography |
| **Security Operations** | Incident response & incident management, root cause analysis, troubleshooting, documentation |
| **Networking** | TCP/IP, DNS, DHCP, routing, firewalls, VPNs, SSH |
| **Scripting & Tools** | Terraform, AWS CLI, PowerShell, Python (basic), Linux command line, Git / GitHub |
| **Operating Systems** | Windows Server, Windows 10/11, Linux, macOS, iOS |

## Cloud Security Projects

### Secure Bastion Host Architecture on AWS | Cloud Security

**Stack:** *Terraform, AWS VPC, Subnets, Route Tables, Internet Gateway, EC2, Security Groups, SSH*

- Provisioned an isolated AWS VPC entirely in Terraform: a public subnet hosting a bastion host (SSH restricted to a single admin IP) and a private subnet with no route to the internet.
- Locked private-instance SSH to the bastion's security group instead of an IP range, so a leaked address cannot reach internal hosts directly.
- Used SSH agent forwarding so private keys are never stored on the bastion; verified real isolation by confirming outbound traffic from the private host times out.

### IAM Privilege Escalation: Exploit & Remediation | Identity & Access

**Stack:** *AWS IAM, AWS CLI, Terraform, S3, JSON policy documents*

- Built a "low-privilege" IAM user with a self-scoped `iam:AttachUserPolicy` permission, then exploited it to attach AdministratorAccess and gain full account control.
- Identified the root cause: any permission letting a principal modify its own access (AttachUserPolicy, PutUserPolicy, CreatePolicyVersion, PassRole) is an escalation path.
- Remediated with a least-privilege policy (read-only on a single S3 bucket) and re-ran the same attack to confirm it was blocked with AccessDenied.

## Certifications

- **AWS Certified Cloud Practitioner (CLF-C02)** | Exam scheduled October 2026
- **AWS Certified AI Practitioner** | In progress

## Professional Experience

### Technical Support & Sales Specialist | Moneris

**July 2023 – Nov 2025** | *Toronto, ON (Hybrid) | Payment processing / fintech*

- Diagnosed and resolved complex merchant payment system issues (terminal configuration, network connectivity, software faults), reducing repeat calls by 15%.
- Escalated backend payment processing failures to engineering with clear root cause documentation, applying a structured, incident-style triage approach.
- Investigated transaction declines, connectivity drops, and hardware malfunctions to isolate root causes across network, device, and software layers.
- Maintained a 91% quality assurance score and ranked top tier for technical resolution accuracy; exceeded monthly sales targets by 40–75%.
- Documented recurring technical issues to strengthen the internal knowledge base and reduce average handling time.

### iPhone & Mac Technical Support Specialist | Concentrix (Apple)

**June 2020 – Jan 2023** | *Remote*

- Provided end-to-end support for macOS and iOS, including system recovery, iCloud account setup, and application troubleshooting, across 500+ inquiries per month.
- Diagnosed hardware and software faults with diagnostic tools and step-by-step methodology, achieving 89% customer satisfaction.
- Tracked issues in CRM tools and flagged recurring problems for internal knowledge sharing.

### Billing & Sales Representative | Cogeco

**Nov 2018 – June 2020** | *Oakville, ON*

- Resolved complex billing, service change, and account adjustment inquiries for TV, internet, and phone; de-escalated disputes and retained at-risk accounts while averaging 20+ new sales monthly.

## Education

### Computer Systems Technician – Cyber Security (Diploma) | Sheridan College

**Expected April 2027** | *Hazel McCallion Campus, Mississauga, ON*

- **Relevant coursework:** Cloud Security & Penetration; Access & Identity Management; Incident Management & Security; MS PowerShell Scripting
- **Grades:** Cryptography 90% • Windows Administration 85% • Cloud Infrastructure (VPC, Subnetting, NACLs) 80% • Network Infrastructure 80%

### Bachelor of Arts – Business Communication (Honours) | Brock University

**April 2017** | *St. Catharines, ON*

## Awards & Community

- Top Technical Agent, Sales Performance (BCR) & Quality Assurance, Moneris (Feb & Mar 2025); Call Flow Excellence, Moneris (June 2025)
- Co-host, Bitcoin Bay (Bitcoin & Lightning Network technology meetup) • Member, OakZen Meditation Group