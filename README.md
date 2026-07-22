# Hey, I'm Luigi (0xBahalaNa)

## About Me

I work at the intersection of **compliance engineering and public safety technology**. My background spans Identity Governance and Administration (privileged access monitoring, user access reviews, RBAC analysis) in regulated financial environments and compliance-focused technical support in a **FedRAMP High** environment serving federal and state/local law enforcement agencies.

I build tools that automate audit evidence collection, continuous monitoring, and compliance-as-code workflows in AWS, replacing manual checkbox processes with repeatable, scriptable, auditor-ready outputs.

**Open to:** GRC Engineer | Compliance / Controls Engineer | IT Controls & Compliance Data Engineer | Identity Governance Engineer

**Centering:** GRC Engineering × Data Engineering × Identity Governance — audit evidence as a data product; identity governance (IGA) as the deepest domain. Federal/public-safety (FedRAMP High, CJIS) is my sharpest *evidence* base, not a constraint on where I'll work.

**Frameworks:** CJIS Security Policy v6.0 | FedRAMP High | NIST 800-53 Rev 5 | NIST CSF 2.0

**Certifications:** SSCP | CySA+ | PenTest+ | Security+

## What I'm Building

These repos form a **compliance lifecycle**: each tool handles a stage of the continuous monitoring and audit evidence pipeline.

```
Audit tools detect -> Config monitor watches -> Remediation fixes
    -> Evidence logger collects -> Compliance report visualizes
    -> Evidence warehouse proves the population is complete (dbt tests + lineage)
    -> OSCAL pipeline produces machine-readable SAR evidence
```

- **GRC Engineering:** automating audit evidence collection and compliance-as-code workflows, mapping tools to CJIS Security Policy, FedRAMP, and NIST 800-53 controls
- **Identity Engineering (IAM/IGA):** streamlining access reviews and provisioning pipelines, applying AC-family control requirements to real infrastructure
- **Cloud Security:** building AWS security tooling aligned to compliance baselines with CI/CD integration

## Technical Stack

| Category | Technologies |
| -- | -- |
| **Cloud** | AWS (CloudTrail, Config, EventBridge, GovCloud, IAM, KMS, Lambda, S3, Security Hub) |
| **Languages** | Python (boto3, oscal-pydantic, compliance-trestle), Bash, AWS CLI, SQL |
| **Data / Analytics Engineering** | dbt, DuckDB, SQL (staging → marts, completeness & reconciliation tests), source data contracts |
| **Infrastructure as Code** | AWS CloudFormation, Terraform |
| **Policy-as-Code** | OPA/Rego, Checkov, Conftest |
| **CI/CD** | GitHub Actions |
| **IAM & IGA** | Access Reviews, Privileged Access Monitoring, RBAC, Least Privilege, SSO |
| **Compliance Frameworks** | CJIS Security Policy v6.0, FedRAMP High, NIST 800-53 Rev 5, NIST CSF 2.0 |
| **Machine-Readable Compliance** | OSCAL (Assessment Results SAR, Component Definitions), IBM Compliance Trestle, oscal-pydantic |
| **Observability** | Kibana/OpenSearch, Splunk, Sentry, SIEM dashboards (KQL) |

## Featured Projects

### Active Flagships

- **[GRC Engineering Evidence Warehouse](https://github.com/0xBahalaNa/evidence-warehouse):** Audit evidence as a data product. Producer audit scripts (S3, SG, CloudTrail, evidence-logger) land as raw records in DuckDB; dbt stages and unifies them into a queryable findings model; dbt tests enforce that the evidence population is **complete and reconciled**, failing loudly instead of degrading silently. The layer *after* the audit scripts run — proving the evidence set is complete, with lineage from API call to finding. v1.0 in development.
- **[IAM Access Review](https://github.com/0xBahalaNa/iam-access-review):** A user access review (UAR) data pipeline — SQL-based population completeness, source reconciliation, and typed exception detection over multi-source identity data, producing an auditor-ready evidence packet. SOX ITGC framing (Access to Programs and Data), crosswalked to NIST 800-53 AC-2/AC-6 and SOC 2 CC6. Design-stage (v1.0 in progress).
- **[OSCAL Evidence Pipeline](https://github.com/0xBahalaNa/oscal-evidence-pipeline):** Transforms compliance findings from existing audit tools into OSCAL Assessment Results (SAR) JSON — the machine-readable evidence format required by FedRAMP 20x and expected by federal assessors. Built on IBM Compliance Trestle and oscal-pydantic. v1.0 in flight.
- **[AWS GRC Terraform Modules](https://github.com/0xBahalaNa/aws-grc-terraform-modules):** Reusable Terraform modules for FedRAMP High and CJIS v6.0 baselines on AWS, with OPA/Rego policy tests and tfsec/checkov CI gates. Each module ships with a `compliance_attestation` output that downstream OSCAL evidence pipelines cite as proof. Companion to the AWS Fundamentals Labs Curriculum on [luigicarpio.dev/blog](https://luigicarpio.dev/blog).

### Frameworks & Gap Analysis

- **[NIST 800-53 Rev 5 to AWS Mapping](https://github.com/0xBahalaNa/nist-800-53-rev-5-to-aws-mapping):** Maps NIST 800-53 Rev 5 controls to AWS services, stored as an OSCAL Component Definition. Generator renders markdown with FedRAMP High baseline filtering and a CJIS v6.0 delta section identifying where CJIS exceeds FedRAMP.
- **[CJIS-FedRAMP Gap Analysis](https://github.com/0xBahalaNa/cjis-fedramp-high-gap-analysis):** Compares CJIS Security Policy v6.0 and FedRAMP High baselines (both aligned to NIST 800-53 Rev 5). Identifies 13 implementation-level deltas and 15 control-level gaps (CJIS-only controls), encoded as an OSCAL overlay.

### Infrastructure & Continuous Monitoring

- **[AWS Compliance as Code](https://github.com/0xBahalaNa/aws-compliance-as-code):** CloudFormation templates and Service Control Policies enforcing security baselines across CJIS, FedRAMP High, and NIST 800-53. Five-layer baseline (CloudTrail + S3 Object Lock + VPC Flow Logs, IAM, KMS CMK, AWS Config, GuardDuty + Security Hub) plus org-level SCPs.
- **[AWS Config Compliance Monitor](https://github.com/0xBahalaNa/aws-config-compliance-monitor):** Event-driven compliance monitoring and auto-remediation for CJIS and FedRAMP High environments using AWS Config, Lambda, and SSM.

### Audit & Evidence Collection Tools

- **[IAM Audit](https://github.com/0xBahalaNa/iam-audit):** Audits AWS IAM users for MFA compliance, access key rotation, and credential hygiene.
- **[S3 Audit](https://github.com/0xBahalaNa/s3-audit):** Audits S3 buckets for encryption, public access, and versioning.
- **[Security Group Audit](https://github.com/0xBahalaNa/sg-audit):** Audits security groups for overly permissive inbound rules.
- **[CloudTrail Audit](https://github.com/0xBahalaNa/cloudtrail-audit):** Audits CloudTrail logs for root account usage, failed API calls, and sensitive IAM / SG / Trail / S3 changes.
- **[Evidence Logger](https://github.com/0xBahalaNa/evidence-logger):** Generates timestamped, auditor-ready evidence files from compliance checks.
- **[Compliance Report](https://github.com/0xBahalaNa/compliance-report):** Aggregates compliance data into structured reports with pass/fail summaries.

### Security & Policy-as-Code

- **[Policy Checker](https://github.com/0xBahalaNa/policy-checker):** Scans AWS IAM policies for overly permissive configurations and CJIS v6.0 violations. 27 unit tests, GitHub Actions CI/CD.
- **[Secret Scanner](https://github.com/0xBahalaNa/secret-scanner):** Scans files and repos for exposed credentials, secrets, and CJI identifiers (ORI, NCIC, FBI numbers, State IDs) with CI/CD gating via non-zero exit codes. Used as the first adapter in [OSCAL Evidence Pipeline](https://github.com/0xBahalaNa/oscal-evidence-pipeline).

> Each tool includes control mappings to NIST 800-53 Rev 5, FedRAMP High, and CJIS Security Policy v6.0 requirements.

## Currently Learning

- **CGE-P (Certified GRC Engineer – Practitioner)** — portfolio in progress ([cge-p-portfolio](https://github.com/0xBahalaNa/cge-p-portfolio)): lab work incl. Cosign keyless chain-of-custody evidence signing and a Terraform GRC CI gate. Targeting the August 2026 window.
- **Terraform module patterns** for FedRAMP High and CJIS v6.0 baselines (per-module OPA/Rego policy bundles, compliance attestation outputs, plan-time validation)
- **OPA / Rego** policy-as-code testing patterns (conftest, plan-time policy gates)
- **CJIS Security Policy v6.0 deltas** from FedRAMP High (FIPS 140-2/3, agency-managed keys, CJI-specific access controls)

## Where to Find Me

[Portfolio](https://luigicarpio.dev) | [LinkedIn](https://www.linkedin.com/in/luigi-carpio) | [Medium](https://medium.com/@0xBahalaNa) | [HackTheBox](https://app.hackthebox.com/public/users/1843403)
