
# AWS SSO & Federated Access Audit Evidence

## Clear, Defensible Evidence for Federated Identity and Role-Based Access in AWS

Single Sign-On (SSO) and federated access fundamentally change how authentication and authorization work in AWS.

Yet this is one of the most commonly misunderstood and under-audited areas of cloud assessments.

Blackbox Auditor produces **clear, defensible audit evidence** for AWS SSO, federated identity, and the role-based permissions that govern access.

---

## Why Federated Access Is Missed in AWS Audits

Traditional audit approaches often assume:

- Users authenticate directly to AWS  
- IAM users represent all access  
- Permissions can be reviewed statically  

These assumptions break down in modern AWS environments.

In reality:
- Access is frequently federated from corporate identity providers  
- Permissions are granted through assumed roles  
- Trust relationships determine *who can become who*  

Without tooling, auditors often miss federated access entirely—or misunderstand its impact.

---

## What Auditors Must Be Able to Answer

A defensible federated access review must clearly show:

- Whether AWS SSO or external identity providers are in use  
- Which users and groups can federate into AWS  
- Which IAM roles can be assumed through federation  
- What permissions those roles grant in practice  
- Whether external identities or accounts have access  

Blackbox Auditor is built to answer these questions directly.

---

## Federated Access Audit Evidence Domains

### AWS SSO and Identity Provider Detection
Blackbox Auditor identifies when federated access is in use.

- AWS SSO enabled or disabled  
- External identity providers configured  
- Federation mechanisms in use  
- Indicators when additional audit procedures are required  

**Suggested screenshot:**  
Overview showing SSO and identity providers detected in the account.

---

### Federated Users, Groups, and Role Mapping
Federated identities do not exist as IAM users.

Blackbox Auditor maps:

- Federated users and groups from identity providers  
- The IAM roles they are permitted to assume  
- The permissions associated with those roles  

This creates a clear lineage from **identity → role → effective permissions**.

**Suggested table:**  
Federated Group | Assumable Role | Effective Privilege Level

---

### Role-Based Permissions and Effective Access
Permissions in federated models are entirely role-driven.

Blackbox Auditor analyzes:

- Policies attached to federated roles  
- Aggregated effective permissions  
- Identification of administrative or high-risk roles  
- Privilege overlap across roles  

Auditors can clearly identify where elevated access exists.

**Suggested screenshot:**  
Effective permissions summary for a federated role.

---

### Cross-Account and External Trust Relationships
Federation often extends beyond a single AWS account.

Blackbox Auditor surfaces:

- Cross-account role trust relationships  
- External AWS accounts trusted for access  
- Roles assumable by external principals  
- Clear visibility into lateral access paths  

This prevents blind spots in multi-account environments.

**Suggested table:**  
Trusted Account | Assumable Role | Access Scope | Risk Indicator

---

## What the Evidence Looks Like

Blackbox Auditor produces:

- Human-readable, auditor-friendly tables  
- Timestamped and reproducible evidence outputs  
- Clear indicators of federated and external access  
- Outputs suitable for walkthroughs and re-performance  

Evidence is designed to withstand peer review and inspection.

---

## Audit Framework Alignment

Federated access evidence supports requirements commonly found in:

- SOC 2 (e.g., CC6.x)  
- PCI DSS (e.g., Req. 7 and 8)  
- ISO 27001 (e.g., Annex A.9)  
- HIPAA Security Rule access controls  

Framework mapping supports—but does not replace—auditor judgment.

---

## Who This Page Is For

- External auditors reviewing AWS SSO and federated identity  
- Internal GRC teams validating access paths  
- Security teams supporting audit evidence requests  

### Not Intended For

- Identity governance lifecycle management  
- Continuous identity threat detection  
- SSO provisioning workflows  

---

## Evaluate Federated Access the Way Auditors Do

- **View Sample Federated Access Evidence**
- **Request a Read-Only Demo**
