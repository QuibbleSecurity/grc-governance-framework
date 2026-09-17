# Case Study: SOC 2 Readiness for a SaaS Platform (Anonymized)

> This case study is a composite/anonymized illustration of a typical engagement structure. Client name, dates, and specific figures have been fictionalized to protect confidentiality.

## Client Profile

A B2B SaaS company (~40 employees) preparing for its first SOC 2 Type II audit at the request of an enterprise prospect. Fully cloud-native, no on-premise infrastructure — access, identity, and audit logging were spread across a fragmented set of point solutions with no single system of record.

## Engagement Scope

- Trust Services Criteria: Security, Availability
- Evidence collection platform: Vanta
- Timeline: 8 weeks from kickoff to audit-ready

## Approach

**Phase 1 — Gap Assessment (Week 1–2)**

Baseline assessment, built from stakeholder interviews (engineering lead, HR, leadership) plus a review of existing policy and evidence, identified 14 control gaps rated Critical / High / Medium by likelihood and impact. The gaps clustered into three themes:

- **Access management** — no org-wide MFA enforcement, no documented offboarding SLA (access to a former contractor's account was found still active three weeks after departure), and default broad access to a shared drive rather than role-scoped provisioning.
- **Vendor & evidence management** — no formal vendor risk review process, and evidence for several controls existed only as informal Slack threads rather than retained, dated artifacts.
- **Monitoring & escalation** — audit logging was enabled but nobody owned reviewing it; there was no defined escalation path from a detected anomaly to an assigned owner.

**Phase 2 — Remediation Roadmap (Week 2–3)**

Gaps were triaged into a roadmap using a risk-rating × effort model, with a fast-track lane for anything that would block the audit outright. Four P0 items were addressed first: org-wide MFA enforcement, a documented incident response plan, a written offboarding SLA with IT/HR ownership assigned, and centralization of identity into a single provider so access could be reviewed and revoked from one place instead of six.

**Phase 3 — Security Awareness Training (Week 3–6, ongoing)**

Org-wide security awareness training was delivered, scoped to a headcount too small for typical enterprise training-platform seat minimums. A quarterly phishing simulation program was established, with results routed into the evidence platform as audit-ready completion records rather than a one-off PDF.

**Phase 4 — Policy Suite (Week 4–7)**

Eleven policies were drafted and approved, each cross-referenced to the specific SOC 2 control(s) it satisfies and loaded into the evidence platform — including, for the first time, formal Onboarding and Offboarding policies with defined SLAs (directly closing the access-management gap identified in Phase 1) and a Role-Based Access Matrix that replaced the prior default-access model.

## Outcome

Client entered its SOC 2 Type II observation window with all P0/P1 gaps closed and automated evidence collection running for ~85% of in-scope controls. The offboarding SLA and access matrix introduced in Phase 4 were later cited by the client as the control they were most surprised hadn't existed already.

## Lessons Applied to the Framework

This engagement is where the "audit-blocking fast-track" prioritization lane in the [Remediation Roadmap methodology](../methodology/four-phase-framework.md) was formalized — smaller clients consistently needed a small set of items resolved immediately rather than worked in strict risk-rank order. It's also why the [Policy Suite](../templates/policy-suite/) now includes dedicated [Onboarding](../templates/policy-suite/onboarding-policy-template.md) and [Offboarding](../templates/policy-suite/offboarding-policy-template.md) policy templates paired with a [Role-Based Access Matrix](../templates/role-based-access-matrix-template.csv) template: access-lifecycle gaps — not just missing technical controls — turned out to be one of the most common and highest-risk findings across engagements.
