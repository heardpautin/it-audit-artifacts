# RBAC Logical Access Testing (Sample Workpaper)

## Objective
Validate that logical access is provisioned according to role-based access control (RBAC) and the principle of least privilege, with appropriate approvals and periodic review.

## Control Statement (Example)
Access to systems and applications is granted based on approved job role, is reviewed periodically, and is removed when no longer required.

## Scope
- In scope: RBAC role assignments for selected systems (see Evidence List)
- Out of scope: application code, infrastructure configuration, physical access

## Evidence Requested
- User-to-role assignment export (CSV)
- Role definition / entitlement mapping (RBAC matrix)
- Approval or ticket evidence for sampled assignments
- Most recent access review/certification evidence (if applicable)

## Sampling Approach
A judgmental sample was selected to prioritize higher-risk roles and access levels:
- Privileged access (admin / elevated roles)
- Write access to sensitive systems
- Roles with segregation-of-duties (SoD) relevance

Sample size: 5–10 role assignments (or as available)

## Test Steps
1. Obtain the user-to-role export and RBAC role definitions.
2. Select a sample of users/roles based on risk (privileged, write, sensitive).
3. For each sampled user/role:
   - Confirm access aligns to stated job role.
   - Confirm approval evidence exists (manager + system owner/security where required).
   - Confirm access level matches least privilege (no excess entitlements).
   - Confirm access is included in periodic review/certification (if the org performs them).
4. Document results and note any exceptions.

## Criteria for Pass/Fail
**Pass** if:
- Role assignment matches job function
- Approval evidence exists and is appropriate
- No excessive access beyond role definition
- Included in periodic review (when required)

**Fail/Exception** if:
- Missing approvals
- Excessive access vs. role definition
- Privileged access not protected (e.g., no MFA/PIM where expected)
- Not reviewed within required interval

## Results Table (Example)
| Sample ID | User/Role | System | Access Level | Approval Present | Review Evidence | Result | Notes |
|---|---|---|---|---|---|---|---|
| S1 | u12345 / Loan Officer | Core Banking | Read/Write | Yes | N/A | Pass | Matches role definition |
| S2 | u67890 / IT Admin | AD/Entra | Privileged | Partial | Yes | Exception | Missing security approval |
| S3 | u24680 / Audit Analyst | Audit Log System | Read Only | Yes | Yes | Pass | Quarterly review confirmed |

## Exceptions & Impact (If Any)
- Exception ID:
- Condition:
- Risk/Impact:
- Recommendation:

## Management Response (Placeholder)
- Owner:
- Target date:
- Corrective action:

## Auditor Notes
This workpaper is for demonstration/lab purposes using simulated or redacted data.
