
# AWS IAM Audit Evidence

## Clear, Defensible Evidence for AWS Identity, Privilege, and Trust

Auditing AWS Identity and Access Management (IAM) is fundamentally different from auditing traditional directory services.

There is no single “admins group.”  
Permissions are inherited, federated, assumed, and distributed across users, roles, access keys, and trust relationships.

Blackbox Auditor produces **clear, defensible IAM audit evidence** that auditors can actually rely on.

---

## Why AWS IAM Audits Fail Without Specialized Tooling

Most AWS IAM audit failures stem from the same issues:

- Overreliance on client-provided access lists  
- Incomplete visibility into access keys and root usage  
- Failure to identify federated and SSO-based access  
- Misinterpretation of role permissions and trust relationships  
- Manual review of JSON policies without effective privilege resolution  

These gaps lead to inaccurate conclusions about who can access AWS and at what level.

---

## What Auditors Need to Answer

An effective IAM audit must clearly and defensibly answer:

- Who can authenticate into AWS?  
- How do they authenticate (password, access key, SSO, federation)?  
- What permissions do they have in practice, not in theory?  
- Which users or roles have administrative or high-risk access?  
- Which external identities or accounts are trusted?  

Blackbox Auditor is designed specifically to answer these questions.

---

## IAM Audit Evidence Domains

### IAM Users, Groups, and Permissions
Blackbox Auditor collects and normalizes IAM user and group data into auditor-ready tables.

- User creation dates, status, and group membership  
- Effective permissions with emphasis on administrative access  
- Identification of stale, inactive, and generic accounts  
- Clear visibility into privilege accumulation  

Auditors no longer need to interpret raw policy documents.

---

### Access Keys and Programmatic Access
Access keys are frequently overlooked during audits, despite their risk.

Blackbox Auditor surfaces:

- All active and inactive access keys  
- Key age, rotation status, and last-used data  
- Identification of long-lived or unused keys  
- Programmatic access paths tied to users and roles  

This evidence allows auditors to assess programmatic access with confidence.

---

### Password Policy, MFA, and Root User Evidence
Critical authentication controls are often reviewed incompletely.

Blackbox Auditor provides:

- AWS account password policy settings  
- MFA enforcement status  
- Root user existence, configuration, and activity  
- Evidence that root access is restricted and monitored  

This ensures root and authentication controls are not excluded from the audit.

---

### AWS SSO and Federated Access Evidence
Federated access is one of the most misunderstood areas of AWS audits.

Blackbox Auditor identifies:

- Whether AWS SSO or external identity providers are in use  
- Federated users and groups with access to AWS  
- Roles assumed through federation  
- Permissions associated with federated access  

The tool highlights when additional audit procedures are required and explains why.

---

### IAM Roles and Trust Relationships
Roles and trust policies define who *can become* someone else in AWS.

Blackbox Auditor analyzes:

- User-assumable roles  
- Cross-account roles  
- Trust relationships between AWS accounts  
- External account access paths  

Complex trust data is simplified into evidence auditors can understand and defend.

---

## What the Evidence Looks Like

Blackbox Auditor produces:

- Normalized, human-readable tables  
- Timestamped, reproducible outputs  
- Evidence aligned to audit workpapers  
- Clear indicators of elevated and administrative access  

Evidence is designed to support walkthroughs, sampling, and re-performance.

---

## Supported Audit Frameworks

IAM audit evidence supports requirements commonly found in:

- SOC 2 (e.g., CC6.x)  
- PCI DSS (e.g., Req. 7 and 8)  
- ISO 27001 (e.g., Annex A.9)  
- HIPAA Security Rule access controls  

Framework mapping is provided without obscuring the underlying evidence.

---

## Who This Is For

- External auditors performing AWS-based assessments  
- Internal GRC teams validating identity and access controls  
- Security teams supporting audit evidence requests  

### Not Intended For

- Real-time identity threat detection  
- Continuous access monitoring  
- Identity governance workflows  

---

## Evaluate IAM Evidence the Way Auditors Do

- **View Sample IAM Audit Evidence**
- **Request a Read-Only Demo**
