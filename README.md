# Hey, I'm Luigi (0xBahalaNa)

## About Me

I work at the intersection of **compliance engineering and public safety technology**. My background spans Identity Governance and Administration (privileged access monitoring, user access reviews, RBAC analysis) in regulated financial environments and compliance-focused technical support in a **FedRAMP High** environment serving federal and state/local law enforcement agencies.

I build tools that automate audit evidence collection, continuous monitoring, and compliance-as-code workflows in AWS, replacing manual checkbox processes with repeatable, scriptable, auditor-ready outputs.

**Open to:** GRC Engineer | Compliance Engineer | Security Analyst roles specializing in public safety technology

**Frameworks:** CJIS Security Policy v6.0 | FedRAMP High | NIST 800-53 Rev 5 | NIST CSF 2.0

**Certifications:** SSCP | CySA+ | PenTest+ | Security+ | Network+ | A+ | Project+ | ITIL 4 Foundations | Linux LPI Essentials

## What I'm Building

These repos form a **compliance lifecycle**: each tool handles a stage of the continuous monitoring and audit evidence pipeline.

```
Audit tools detect -> Config monitor watches -> Remediation fixes
    -> Evidence logger collects -> Compliance report visualizes
```

- **GRC Engineering:** automating audit evidence collection and compliance-as-code workflows, mapping tools to CJIS Security Policy, FedRAMP, and NIST 800-53 controls
- **Identity Engineering (IAM/IGA):** streamlining access reviews and provisioning pipelines, applying AC-family control requirements to real infrastructure
- **Cloud Security:** building AWS security tooling aligned to compliance baselines with CI/CD integration

## Technical Stack

| Category | Technologies |
| -- | -- |
| **Cloud** | AWS (CloudTrail, Config, EventBridge, GovCloud, IAM, KMS, Lambda, S3, Security Hub) |
| **Languages** | Python (boto3, oscal-pydantic, compliance-trestle), Bash, AWS CLI |
| **Infrastructure as Code** | AWS CloudFormation, Terraform |
| **Policy-as-Code** | OPA/Rego, Checkov, Conftest |
| **CI/CD** | GitHub Actions |
| **IAM & IGA** | Access Reviews, Privileged Access Monitoring, RBAC, Least Privilege, SSO |
| **Compliance** | CJIS Security Policy v6.0, FedRAMP High, NIST 800-53 Rev 5, NIST CSF 2.0, OSCAL |
| **Observability** | Kibana/OpenSearch, Splunk, Sentry, SIEM dashboards (KQL) |

## Featured Projects

### Frameworks & Gap Analysis

- **[NIST 800-53 Rev 5 to AWS Mapping](https://github.com/0xBahalaNa/nist-800-53-rev-5-to-aws-mapping):** Maps NIST 800-53 Rev 5 controls to AWS services, stored as an OSCAL Component Definition. Generator renders markdown with FedRAMP High baseline filtering and a CJIS v6.0 delta section identifying where CJIS exceeds FedRAMP.
- **[CJIS-FedRAMP Gap Analysis](https://github.com/0xBahalaNa/cjis-fedramp-gap-analysis):** Compares CJIS Security Policy v6.0 and FedRAMP High baselines (both aligned to NIST 800-53 Rev 5). Identifies 13 implementation-level deltas and 15 control-level gaps (CJIS-only controls), encoded as an OSCAL overlay.

### Infrastructure & Continuous Monitoring

- **[AWS Compliance as Code](https://github.com/0xBahalaNa/aws-compliance-as-code):** CloudFormation templates and Service Control Policies enforcing security baselines
- **[AWS Config Compliance Monitor](https://github.com/0xBahalaNa/aws-config-compliance-monitor):** Event-driven compliance monitoring and auto-remediation for CJIS and FedRAMP High environments using AWS Config, Lambda, and SSM

### Audit & Evidence Collection Tools

- **[IAM Audit](https://github.com/0xBahalaNa/iam-audit):** Audits AWS IAM users for MFA compliance and credential hygiene
- **[S3 Audit](https://github.com/0xBahalaNa/s3-audit):** Audits S3 buckets for encryption, public access, and versioning
- **[Security Group Audit](https://github.com/0xBahalaNa/sg-audit):** Audits security groups for overly permissive inbound rules
- **[CloudTrail Audit](https://github.com/0xBahalaNa/cloudtrail-audit):** Audits CloudTrail configuration for logging compliance
- **[Evidence Logger](https://github.com/0xBahalaNa/evidence-logger):** Generates timestamped, auditor-ready evidence files from compliance checks
- **[Compliance Report](https://github.com/0xBahalaNa/compliance-report):** Aggregates compliance data into structured reports with pass/fail summaries

### Security & Policy-as-Code

- **[Policy Checker](https://github.com/0xBahalaNa/policy-checker):** Scans AWS IAM policies for overly permissive configurations and CJIS v6.0 violations. 27 unit tests, GitHub Actions CI/CD.
- **[Secret Scanner](https://github.com/0xBahalaNa/secret-scanner):** Scans files and repos for exposed credentials and secrets with CI/CD gating via non-zero exit codes

> Each tool includes control mappings to NIST 800-53 Rev 5, FedRAMP High, and CJIS Security Policy v6.0 requirements.

## Currently Learning

- OSCAL and IBM Compliance Trestle for machine-readable compliance artifacts (FedRAMP 20x alignment)
- Terraform for multi-environment IaC deployments
- Open Policy Agent (OPA) and Rego for policy-as-code enforcement
- CJIS Security Policy v6.0 deltas from FedRAMP High (FIPS 140-2/3, agency-managed keys, CJI-specific access controls)

## Where to Find Me

[Portfolio](https://luigicarpio.dev) | [LinkedIn](https://www.linkedin.com/in/luigi-carpio) | [Medium](https://medium.com/@0xBahalaNa) | [HackTheBox](https://app.hackthebox.com/public/users/1843403)