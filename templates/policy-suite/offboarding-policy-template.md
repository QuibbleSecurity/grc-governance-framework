# [Client Name] — Offboarding Policy

## Policy Information

| Field | Value |
|---|---|
| Document Number | HR-POL-[XXX] |
| Effective Date | [Date] |
| Last Updated | [Date] |
| Approval Authority | [Title, e.g., CEO / Head of People] |
| Related Policies | [Cybersecurity & Acceptable Use Policy]; [BYOD Policy]; [Onboarding Policy] |
| Framework Mapping | [e.g., SOC 2 CC6.1, CC6.3 / ISO 27001 A.9.2.6] |

## 1. Purpose

This policy establishes a structured, documented, and auditable process for managing personnel departures — voluntary or involuntary, employee or contractor — to ensure access to [Client Name] systems and data is revoked in a timely, complete, and evidenced manner. It formalizes any existing offboarding checklist into binding policy with defined ownership and timelines.

## 2. Scope

This policy applies to all full-time employees, part-time employees, contractors, advisors, interns, and third-party personnel who hold any credential, device, or access to [Client Name] systems, applications, or data, regardless of the reason for departure.

## 3. Roles & Responsibilities

| Role | Owns |
|---|---|
| HR | Departure documentation, legal review coordination, payroll/benefits deactivation, evidence logging |
| IT / Security Administrator | Identity, MFA, repository/infrastructure, hardware, and MDM/BYOD revocation |
| Finance | Removal from financial systems and privileged financial workflows |
| Manager | Project and role handover to ensure operational continuity |

## 4. Offboarding Timelines & Service-Level Targets

- **Core directory access** must be disabled within **[e.g., 2 hours]** of the offboarding trigger — the earlier of the departure notification (voluntary) or the termination decision (involuntary). For involuntary or for-cause terminations, access must be disabled **before or at the moment** the employee is notified, not after.
- **Privileged financial system access** (Section 7) must begin revocation the same business day and be completed within the timeline defined in Section 7, given its operational sensitivity.
- **All other checklist items** should be completed within **[e.g., 5 business days]** of the departure date, with evidence of completion logged per Section 8.2.

## 5. Phase I — Immediate Actions (Day 1 of Notice)

- **Notification & documentation.** HR formally records the departure date, reason for leaving, and key timelines as soon as notice is received or a termination decision is made.
- **HR & Legal review.** HR and Legal identify whether any specific termination protocols, notice-period obligations, or legal requirements apply.
- **Access audit readiness.** IT pulls the individual's current access roster from the identity provider and the Role-Based Access Matrix to produce a complete list of every system, application, and credential assigned to the individual before revocation begins.

## 6. Phase II — Identity, Access & Hardware Revocation

- **Central directory termination.** IT terminates the individual's user status in the core directory, blocking authentication, within the SLA defined in Section 4.
- **MFA & session revocation.** IT revokes all associated MFA enrollments and clears persistent sessions across SSO-connected platforms.
- **Repository & infrastructure access removal.** IT removes the individual's permissions from project tracking systems, source control, and document repositories, using the access roster from Section 5 to confirm nothing is missed.
- **Hardware recovery.** IT and the individual's manager coordinate recovery of all corporate-issued physical workstations and devices.
- **BYOD handling.** For any personal device enrolled under the BYOD policy, IT performs a selective wipe of the corporate container and de-enrolls the device from MDM. A full-device wipe is not performed absent the circumstances and consent described in that policy.

## 7. Phase III — Financial Controls

- **Signatory & authorization removal.** Finance removes the individual as an authorized user or signatory on corporate payment platforms and banking portals, same business day as the offboarding trigger.
- **Corporate credit facilities.** Finance cancels any active physical or virtual corporate credit cards assigned to the individual.
- **Privileged financial or custodial system access.** Where the departing individual holds elevated access to a sensitive financial, treasury, or custodial system, revocation (including any required credential or key rotation) is initiated immediately upon notice for involuntary departures and completed before the individual's final day of access under any circumstance. A delay that leaves such a system under-provisioned or in a degraded-control state is treated as a security incident.
- **Payroll & benefits deactivation.** HR and Finance coordinate with payroll operators to process final pay cycles and ensure compliance with applicable withholding requirements.

## 8. Phase IV — Governance & Knowledge Management

- **Roles & project handover.** The departing individual's manager transitions ongoing project responsibilities and institutional knowledge to designated team members.
- **Evidence logging.** HR documents the offboarding execution, including final checklist completion timestamps and relevant system logs, in the centralized compliance repository, consistent with the evidence standards applied to onboarding.

## 9. Special Circumstances — Involuntary or For-Cause Departures

For involuntary terminations, terminations for cause, or any departure assessed as elevated-risk (including departures of personnel with production, financial, or privileged system access), all Phase II and Phase III actions should be accelerated to the maximum extent operationally possible: access disabled at or before the moment of notification rather than afterward, hardware recovery coordinated as an escorted same-day collection where feasible, and any required credential/key rotation initiated immediately rather than on the standard same-business-day timeline.

## 10. Enforcement

Failure to complete offboarding actions within the timelines defined in this policy is treated as a control failure and must be escalated to HR and Security leadership. Repeated or systemic delays are documented and addressed as part of the organization's continuous monitoring program.

## 11. Policy Administration

HR and IT jointly own this policy. IT and Finance review the offboarding SLA and any privileged-system revocation procedures on a defined cadence (e.g., annually), or upon any material change to the organization's identity, financial, or infrastructure stack.

---

## Appendix A — Offboarding Checklist

To be completed per departure and retained as offboarding evidence. "Target" reflects the timeline defined in Section 4; involuntary/for-cause departures follow Section 9's accelerated timelines instead.

**Phase I — Immediate Actions (Day 1 of Notice)**

| Task | Owner | Target | Done | Date |
|---|---|---|---|---|
| Record departure date, reason for leaving, and key timelines | HR | Day 1 | ☐ | |
| Identify applicable termination protocols or legal obligations | HR / Legal | Day 1 | ☐ | |
| Pull current access roster from identity provider / Access Matrix | IT | Day 1 | ☐ | |

**Phase II — Identity, Access & Hardware Revocation**

| Task | Owner | Target | Done | Date |
|---|---|---|---|---|
| Terminate user status in core directory | IT | Within SLA | ☐ | |
| Revoke MFA tokens; clear persistent sessions | IT | Within SLA | ☐ | |
| Remove access from project tracking, source control, document repositories | IT | Within SLA | ☐ | |
| Recover corporate-issued hardware | IT + Manager | 5 business days | ☐ | |
| Selective wipe of corporate container on BYOD device(s) | IT | Within SLA | ☐ | |
| De-enroll device(s) from MDM | IT | 5 business days | ☐ | |

**Phase III — Financial Controls**

| Task | Owner | Target | Done | Date |
|---|---|---|---|---|
| Remove signatory / authorized-user status on banking platforms | Finance | Same business day | ☐ | |
| Cancel active physical/virtual corporate credit cards | Finance | Same business day | ☐ | |
| Revoke/rotate access to privileged financial or custodial systems | Finance / IT | Immediate – before final access | ☐ | |
| Coordinate final pay cycle and benefits deactivation | HR + Finance | 5 business days | ☐ | |

**Phase IV — Governance & Knowledge Management**

| Task | Owner | Target | Done | Date |
|---|---|---|---|---|
| Transition project responsibilities to designated team member(s) | Manager | 5 business days | ☐ | |
| Log offboarding completion timestamp and system logs centrally | HR | 5 business days | ☐ | |

