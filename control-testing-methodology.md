# Control Testing Methodology

## Purpose
This document describes the methodology used to evaluate the design and operating effectiveness of controls within IT environments. Control testing is performed to validate that controls are functioning as intended, align with defined policies and risk tolerances, and provide evidence supporting audit conclusions.

---

## 1. Control Identification
Controls subject to testing are identified based on:
- Organizational risk profile
- Audit scope and objectives
- Regulatory and compliance criteria (e.g., ISO 27001, NIST 800-53/800-171)
- Framework mappings (e.g., COBIT, COSO)

Example control categories include:
- Logical access controls
- Privileged account management
- Change management
- Backup and recovery controls
- Physical access controls

---

## 2. Control Design Evaluation
For each control identified:
- Assess whether the control is **defined** in policy or procedure
- Confirm the control owner and responsible party
- Determine whether the control has clear expectations
- Evaluate whether the control’s design would mitigate risk if operating as intended

Criteria for design evaluation:
- Alignment to policy/standard
- Completeness of criteria
- Relevance to key risk areas

---

## 3. Evidence Acquisition
Evidence is acquired to support both design and operating effectiveness tests. Evidence may include:
- System outputs (logs, reports, exports)
- Configuration screenshots / settings
- Access provisioning tickets
- Approval workflows
- Review certs and sign-offs
- Role/entitlement matrices

Evidence must be:
- Time-bound (date/time stamped)
- Source verifiable
- Relevant to the control being tested

---

## 4. Sampling Approach
Given large populations, sampling is used to provide reasonable assurance.

Sampling principles:
- Risk-based: prioritize high-impact and high-likelihood areas
- Sufficient: sample size adequate for conclusion
- Representative: covers variety of scenarios

Sampling may include:
- Privileged accounts
- Elevated permissions
- Recently onboarded/moved users
- Accounts with SoD conflicts

---

## 5. Test Execution
For each control and sample item:
1. Retrieve evidence
2. Compare actual state to expected control criteria
3. Document findings
4. Note exceptions and potential impact

Key execution checks:
- Access aligns to defined role
- Approval evidence exists
- Required periodic reviews occurred
- Technical enforcement matches policy requirements

---

## 6. Exception Handling
An exception exists when evidence indicates the control is:
- Not operating as intended
- Missing key attributes
- Ineffective in practice

Steps on exception:
- Document condition and criteria
- Categorize severity (Low/Med/High)
- Assess business impact
- Draft exception record

Exceptions do NOT include:
- Missing evidence due to scope limitations
- Non-relevant items outside defined audit boundaries

---

## 7. Conclusion and Reporting
After testing:
- Summarize results
- Highlight areas of non-compliance
- Provide context on control maturity
- Submit to appropriate stakeholders

Typical deliverables:
- Workpapers
- Exception listings
- Executive summaries
- Management responses

---

## 8. Documentation and Versioning
All test artifacts are maintained within the audit repository with:
- Clear timestamps
- Version history
- Linked source evidence
- Auditable trail

This supports reproducibility and traceability and aligns with quality and compliance expectations.
