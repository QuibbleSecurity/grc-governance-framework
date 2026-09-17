# [Client Name] — Onboarding Policy

## Policy Information

| Field | Value |
|---|---|
| Document Number | HR-POL-[XXX] |
| Effective Date | [Date] |
| Last Updated | [Date] |
| Approval Authority | [Title, e.g., CEO / Head of People] |
| Related Policies | [Cybersecurity & Acceptable Use Policy]; [BYOD Policy]; [Offboarding Policy] |
| Framework Mapping | [e.g., SOC 2 CC6.1, CC6.2 / ISO 27001 A.6.1, A.9.2] |

> This policy formalizes [Client Name]'s onboarding practice into a documented, repeatable, and auditable process, and establishes the Role-Based Access Matrix ([Appendix B](../role-based-access-matrix-template.csv)) as the sole authorized basis for provisioning system access — replacing any prior default of broad, unrestricted access.

## 1. Purpose

This policy defines the required security, access-provisioning, contractual, and training steps that must be completed before and during the first period of any new employee's or contractor's engagement with [Client Name].

## 2. Scope

This policy applies to all full-time employees, part-time employees, contractors, advisors, interns, and third-party personnel who will be granted access to any [Client Name] system, account, or data, regardless of whether that access is provisioned by IT, HR, or a functional lead.

## 3. Roles & Responsibilities

| Role | Owns |
|---|---|
| HR | Background checks, contractual execution, policy acknowledgment tracking, Week 1 training documentation |
| IT / Security Administrator | Identity provisioning, MDM enrollment, MFA enforcement, system access provisioning per the Role-Based Access Matrix |
| Hiring Manager | Confirms the new hire's role and corresponding access tier before Day 1; requests any role-specific exceptions in writing |
| New Hire / Contractor | Completes required acknowledgments and training within the timelines defined below |

## 4. Phase 1 — Pre-Onboarding (Clearance & Governance)

Before any employee or contractor is granted access to the environment or any sensitive data system, the following must be fully executed:

- **Background screening.** A background check is required for every incoming full-time employee and independent contractor prior to any system access being granted. Where talent is sourced through a staffing agency, the underlying contract must explicitly require the agency to perform this check prior to assignment. Completed certificates are filed in the secure HR repository.
- **Contractual execution.** Full-time employees: the employment agreement is fully executed prior to Day 1. Contractors/advisors: a signed agreement with an appropriate confidentiality schedule (or Business Associate Agreement, where applicable) is in place before any technical infrastructure or data access is authorized.

## 5. Phase 2 — Day 1 (Identity Provisioning & Access Configuration)

- **Device management.** All active workstations are enrolled immediately in the organization's MDM platform. A minimum supported OS/edition baseline is enforced (e.g., no unmanaged "Home" editions on corporate-issued Windows devices).
- **MFA enforcement.** Multi-factor authentication is enforced at initial login and required without exception across the identity provider, source control, and all business-critical SaaS platforms.
- **Access provisioning.** System access is provisioned strictly according to the new hire's role, as defined in the [Role-Based Access Matrix](../role-based-access-matrix-template.csv). Default, unrestricted access to shared drives or any other system is prohibited. Access beyond a role's defined baseline requires written approval from the hiring manager and IT, documented and retained as evidence.
- **Security baseline verification.** Endpoint protection is confirmed active; local disk encryption is confirmed enabled and reporting telemetry to the MDM console.
- **Policy acknowledgments.** New hires electronically sign and acknowledge, tracked in the evidence/compliance platform: Employee Handbook, Code of Conduct, Acceptable Use Policy, and (where applicable) an AI Systems Usage Policy.

## 6. Phase 3 — Week 1 (Training & Continuous Monitoring Transition)

- **Security awareness training.** New team members complete the Information Security Awareness Training module within their first week, including any tool- or role-specific modules (e.g., approved AI tool usage).
- **Sanctions acknowledgment.** The new hire reviews and acknowledges the policy governing security infractions, including how violations are tracked, evaluated, and resolved.
- **Transition to continuous monitoring.** Upon completion of Week 1, the workstation transitions into the automated monitoring queue (patch status, antivirus state, configuration baseline) and is added to the recurring compliance track (annual re-acknowledgment, unannounced phishing simulations).

## 7. Contractor & Third-Party Onboarding

Contractors and third-party personnel follow the same Pre-Onboarding and Day 1 requirements as employees, with two additional constraints:

- Access is provisioned per the Contractor row of the Role-Based Access Matrix rather than by functional role.
- All access is time-limited to the term of the engagement, subject to review if extended, and revoked immediately upon completion per the [Offboarding Policy](offboarding-policy-template.md).

## 8. Enforcement

Provisioning access outside of this policy or the Role-Based Access Matrix without documented approval is treated as a policy violation and may result in access revocation, mandatory retraining, and escalation to HR and Security leadership.

## 9. Policy Administration

HR and IT jointly own this policy. IT maintains the Role-Based Access Matrix and reviews it on a defined cadence (e.g., quarterly), or upon any material change to the organization's system stack or org structure. This policy should be reviewed periodically alongside related security, BYOD, and offboarding policies.

---

## Appendix A — Onboarding Checklist

To be completed per new hire and retained as onboarding evidence.

**Phase 1 — Pre-Onboarding**

| Task | Owner | Done | Date |
|---|---|---|---|
| Initiate background check (employee or contractor) | HR | ☐ | |
| If agency-sourced, confirm contract requires agency-performed background check | HR / Legal | ☐ | |
| File background check certificate in secure HR folder | HR | ☐ | |
| Execute employment / contractor agreement (+ confidentiality schedule or BAA where applicable) | HR | ☐ | |
| Confirm role and access tier per Role-Based Access Matrix | Manager + IT | ☐ | |

**Phase 2 — Day 1**

| Task | Owner | Done | Date |
|---|---|---|---|
| Provision corporate identity | IT | ☐ | |
| Enroll corporate device in MDM | IT | ☐ | |
| Verify device meets minimum OS/edition baseline | IT | ☐ | |
| Enforce MFA enrollment at first login | IT | ☐ | |
| Provision system access per Role-Based Access Matrix (no default broad access) | IT + Manager | ☐ | |
| Verify endpoint protection active and disk encryption enabled | IT | ☐ | |
| New hire signs required policy acknowledgments | HR | ☐ | |
| Log all signed acknowledgments in compliance platform | HR | ☐ | |

**Phase 3 — Week 1**

| Task | Owner | Done | Date |
|---|---|---|---|
| Complete Information Security Awareness Training | New Hire | ☐ | |
| Review and acknowledge sanctions / violations policy | New Hire | ☐ | |
| Confirm workstation added to continuous monitoring queue | IT | ☐ | |
| Add employee to recurring compliance track | HR | ☐ | |

## Appendix B — Role-Based Access Matrix

See [`role-based-access-matrix-template.csv`](../role-based-access-matrix-template.csv) for the baseline access-tier matrix referenced throughout this policy. This is a starting baseline; department leads should validate and adjust role assignments before formal adoption, and any deviation should be documented as an approved exception per Section 5.

