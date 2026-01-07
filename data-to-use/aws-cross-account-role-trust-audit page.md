
# AWS Cross-Account Role & Trust Audit Evidence

## Clear, Defensible Evidence for Cross-Account Access and Trust Relationships in AWS

Cross-account access is a core AWS design pattern.  
It is also one of the least understood and most frequently under-audited areas of cloud environments.

Trust policies, not network boundaries, determine which external accounts, users, or roles can access AWS resources.

Blackbox Auditor produces **clear, defensible audit evidence** for cross-account roles and trust relationships so auditors can accurately assess access risk and scope.

---

## Why Cross-Account Access Is Commonly Missed in Audits

Many audits incorrectly assume:

- Access is limited to a single AWS account  
- Network boundaries define trust  
- IAM users represent all access paths  

In reality:
- AWS accounts frequently trust other AWS accounts  
- Roles can be assumed without local IAM users  
- Trust relationships often extend across environments, subsidiaries, or third parties  

Without specialized tooling, auditors often fail to identify who outside the account can gain access.

---

## What Auditors Must Be Able to Defend

A defensible cross-account review must clearly answer:

- Which external AWS accounts are trusted?  
- Which roles can those accounts assume?  
- What permissions do those roles grant in practice?  
- Are there administrative or high-risk cross-account access paths?  
- Does cross-account access impact audit scope or boundary definitions?  

Blackbox Auditor is built to answer these questions explicitly.

---

## Cross-Account Trust Audit Evidence Domains

### Cross-Account Role Identification
Blackbox Auditor identifies all roles that can be assumed by external AWS accounts.

- Roles trusted by one or more external AWS accounts  
- Trust policy conditions and restrictions  
- Identification of overly broad trust relationships  

Auditors gain immediate visibility into external access paths.

**Suggested table:**  
Trusted AWS Account | Assumable Role | Trust Conditions

---

### Effective Permissions of Cross-Account Roles
Trust alone does not define risk. Permissions do.

Blackbox Auditor analyzes:

- Policies attached to cross-account roles  
- Aggregated effective permissions  
- Identification of administrative or sensitive access  
- Privilege scope across services and resources  

Auditors can clearly see what an external account can actually do.

**Suggested screenshot:**  
Effective permission summary for a cross-account role.

---

### Bidirectional Trust and Lateral Access
Cross-account access is often bidirectional.

Blackbox Auditor highlights:

- Roles this account can assume in other AWS accounts  
- Lateral movement paths across environments  
- Trust relationships that may impact segregation of duties  

This helps auditors evaluate risk across multi-account architectures.

**Suggested table:**  
Source Account | Target Account | Assumable Role | Access Scope

---

### Third-Party and Vendor Access
Cross-account trust is frequently used to grant vendor or partner access.

Blackbox Auditor identifies:

- Third-party AWS accounts with access  
- Roles intended for vendor use  
- Permissions granted to external service providers  
- Access paths requiring contractual or compensating controls  

Auditors can verify that third-party access aligns with policy and agreements.

---

## What the Evidence Looks Like

Blackbox Auditor produces:

- Normalized, human-readable trust summaries  
- Timestamped and reproducible evidence  
- Clear indicators of external and lateral access  
- Outputs suitable for walkthroughs, sampling, and re-performance  

Evidence is designed to support defensible audit conclusions.

---

## Audit Framework Alignment

Cross-account access evidence supports requirements commonly found in:

- SOC 2 (e.g., CC6.x, CC7.x)  
- PCI DSS (e.g., Req. 7 and 12)  
- ISO 27001 (e.g., Annex A.9 and A.13)  
- HIPAA Security Rule access controls  

Framework mapping supports audit execution without obscuring technical reality.

---

## Who This Page Is For

- External auditors reviewing AWS multi-account environments  
- Internal GRC teams validating trust boundaries  
- Security teams supporting audit scope and access reviews  

### Not Intended For

- Continuous cloud threat monitoring  
- Identity governance lifecycle management  
- Network segmentation design  

---

## Evaluate Cross-Account Trust the Way Auditors Do

- **View Sample Cross-Account Trust Evidence**
- **Request a Read-Only Demo**
