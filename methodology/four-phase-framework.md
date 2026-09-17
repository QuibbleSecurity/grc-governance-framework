# The Four-Phase GRC Engagement Framework

This is the core service methodology behind every Quibble Security compliance engagement. It's designed to be **platform-agnostic** (works whether the client uses Vanta, Drata, OneTrust, AuditBoard, or nothing at all) and **framework-agnostic** (the phases are the same whether the target is SOC 2, HIPAA, NIST CSF, or GLBA Safeguards Rule — only the control set changes).

## Phase 1 — Gap Assessment

**Goal:** Establish an honest, evidence-based baseline of the client's current control environment against the target framework.

**Inputs:**
- Kickoff questionnaires, one per functional area ([templates](../templates/questionnaires/)): [Executive Leadership](../templates/questionnaires/executive-leadership-questionnaire-template.md), [IT/Systems](../templates/questionnaires/it-systems-questionnaire-template.md), [Finance & Operations](../templates/questionnaires/finance-operations-questionnaire-template.md), and [People/HR](../templates/questionnaires/people-hr-questionnaire-template.md) — sent ahead of kickoff so interviews build on written answers instead of starting cold
- Stakeholder interviews (IT/engineering lead, HR, leadership) to follow up on questionnaire responses
- Existing policy and evidence review

**Outputs:**
- Scored gap assessment report ([template](../templates/gap-assessment-report-template.md)) — control-by-control status (Met / Partially Met / Not Met / N/A), risk rating, and supporting notes
- Populated control matrix ([template](../templates/control-matrix-template.csv))

**Typical duration:** 1–3 weeks depending on scope and framework.

## Phase 2 — Remediation Roadmap

**Goal:** Convert assessment findings into a prioritized, resourced plan the client can actually execute.

**Inputs:** Phase 1 gap assessment output.

**Outputs:**
- Remediation roadmap ([template](../templates/remediation-roadmap-template.md)) — each gap mapped to a remediation action, owner, effort estimate, priority, and target date
- Technical findings routed to a technical remediation partner where applicable (e.g., infrastructure hardening, endpoint deployment)

**Prioritization model:** risk rating × effort, with a fast-track lane for anything that blocks audit readiness (e.g., missing MFA, no incident response plan).

## Phase 3 — Security Awareness Training

**Goal:** Close the human-layer gap that technical and policy controls alone don't cover.

**Outputs:**
- Role-based training session or annual lunch-and-learn
- Quarterly phishing simulation campaign
- Training completion evidence suitable for audit (attendance logs, simulation results)

This phase is scoped to fit organizations too small for typical enterprise training platform seat minimums — a common gap in the 10–50 employee range.

Also available as a standalone 12-month program, independent of the full four-phase engagement — see the [Security Awareness Training Program](../service-offerings/security-awareness-training-program.md) overview for the full rollout structure and deliverables.

## Phase 4 — Tailored Policy Suite

**Goal:** Deliver a policy set that's actually mapped to the target framework's control requirements and reflects how the client really operates — not generic boilerplate.

**Outputs:**
- Core policy set ([templates](../templates/policy-suite/)): Information Security Policy, Acceptable Use Policy, Incident Response Policy, Onboarding Policy, Offboarding Policy, plus framework-specific additions as needed
- A [Role-Based Access Matrix](../templates/role-based-access-matrix-template.csv) establishing the authorized baseline for system access by role — referenced by both the Onboarding and Offboarding policies rather than left as an undocumented default
- Each policy cross-referenced to the control(s) it satisfies in the control matrix

Access-lifecycle management (onboarding provisioning and offboarding revocation, each with defined SLAs) is one of the most common gap categories found in Phase 1 — see the [example engagement case study](../case-studies/example-soc2-readiness-engagement.md) — which is why it now has dedicated templates rather than being folded into a general security policy.

## How the phases connect

```
Gap Assessment  →  Remediation Roadmap  →  Awareness Training  +  Policy Suite
   (baseline)          (the plan)              (ongoing operational controls)
```

Phases 3 and 4 typically run in parallel once the roadmap is approved. For clients using continuous-monitoring platforms (Vanta, Drata), evidence collected in Phases 3–4 is wired into automated control monitoring — see [compliance-as-code-toolkit](../../compliance-as-code-toolkit) for the automation patterns used to validate and monitor that evidence.

