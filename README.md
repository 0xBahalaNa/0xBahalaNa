# Hey, I'm Luigi (0xBahalaNa) 🤝

## About Me

I work at the intersection of **compliance engineering and public safety technology**. My background spans Identity Governance and Administration (privileged access monitoring, user access reviews, RBAC analysis) in regulated financial environments and hands-on technical support in a **FedRAMP High** environment serving federal and state/local law enforcement agencies.

I build tools that automate audit evidence collection and compliance workflows in AWS — replacing manual checkbox processes with repeatable, scriptable, auditor-ready outputs.

**Open to:** GRC Engineer · Compliance Engineer · Security Analyst roles — specializing in public safety technology

**Frameworks I work with:** CJIS Security Policy v6.0 · FedRAMP High · NIST 800-53 Rev 5

**Certifications:** SSCP · CySA+ · PenTest+ · Security+ · Network+ · A+ · Project+ · ITIL 4 Foundations · Linux LPI Essentials

## What I'm Building

These repos form a **compliance lifecycle** — each tool handles a stage of the continuous monitoring and audit evidence pipeline:

```
Audit tools detect → Config monitor watches → Remediation fixes
    → Evidence logger collects → Compliance report visualizes
```

- **GRC Engineering** — automating audit evidence collection and compliance workflows, mapping tools to CJIS Security Policy, FedRAMP, and NIST 800-53 controls
- **Identity Engineering (IAM/IGA)** — streamlining access reviews and provisioning pipelines, applying AC-family control requirements to real infrastructure
- **Cloud Security** — building AWS security tooling aligned to compliance baselines

## Technical Stack

| Category | Technologies |
| --- | --- |
| **Cloud** | AWS (primary) · FedRAMP High / GovCloud context |
| **Languages** | Python, Bash, AWS CLI |
| **Infrastructure as Code** | AWS CloudFormation, Terraform (learning) |
| **Policy-as-Code** | OPA/Rego (learning), Checkov (learning), Conftest (learning) |
| **IAM & IGA** | Access Reviews, Privileged Access Monitoring, RBAC, Least Privilege, SSO |
| **Compliance** | CJIS Security Policy v6.0, FedRAMP High, NIST 800-53 Rev 5 |

## Featured Projects

### ☁️ Infrastructure & Continuous Monitoring

- **[AWS Compliance as Code](https://github.com/0xBahalaNa/aws-compliance-as-code)** — CloudFormation templates and Service Control Policies enforcing security baselines `SC-7 · AC-3 · AU-2`
- **[AWS Config Compliance Monitor](https://github.com/0xBahalaNa/aws-config-compliance-monitor)** — event-driven compliance monitoring and auto-remediation for CJIS and FedRAMP High environments using AWS Config, Lambda, and SSM `CA-7 · SI-4 · CM-3`

### 🐍 Audit & Evidence Collection Tools

- **[IAM Audit](https://github.com/0xBahalaNa/iam-audit)** — audits AWS IAM users for MFA compliance and credential hygiene `IA-2 · AC-2`
- **[S3 Audit](https://github.com/0xBahalaNa/s3-audit)** — audits S3 buckets for encryption, public access, and versioning `SC-28 · AC-3 · SC-13`
- **[Security Group Audit](https://github.com/0xBahalaNa/sg-audit)** — audits security groups for overly permissive inbound rules `SC-7 · AC-4`
- **[CloudTrail Audit](https://github.com/0xBahalaNa/cloudtrail-audit)** — audits CloudTrail configuration for logging compliance `AU-2 · AU-3 · AU-12`
- **[Evidence Logger](https://github.com/0xBahalaNa/evidence-logger)** — generates timestamped, auditor-ready evidence files from compliance checks `AU-6 · CA-2`
- **[Compliance Report](https://github.com/0xBahalaNa/compliance-report)** — aggregates compliance data into structured reports with pass/fail summaries `CA-7 · CA-2`

### 🔒 Security Tooling

- **[Policy Checker](https://github.com/0xBahalaNa/policy-checker)** — scans AWS IAM policies for overly permissive configurations `AC-6 · AC-3`
- **[Secret Scanner](https://github.com/0xBahalaNa/secret-scanner)** — scans files and repos for exposed credentials and secrets `IA-5 · SC-28`

> 🔄 **In progress:** Each tool is being updated with control mappings to NIST 800-53 Rev 5, FedRAMP High, and CJIS Security Policy v6.0 requirements.

## Currently Learning

- OSCAL and IBM Compliance Trestle for machine-readable compliance artifacts (FedRAMP 20x alignment)
- Terraform for multi-environment IaC deployments
- Open Policy Agent (OPA) and Rego for policy-as-code enforcement
- CJIS Security Policy v6.0 deltas from FedRAMP High (FIPS 140-2/3, agency-managed keys, CJI-specific access controls)

## Where to Find Me

[LinkedIn](https://www.linkedin.com/in/luigi-carpio) · [Medium](https://medium.com/@0xBahalaNa) · [HackTheBox](https://app.hackthebox.com/public/users/1843403)