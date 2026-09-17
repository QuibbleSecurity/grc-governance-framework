# The Four-Phase GRC Engagement Framework

This is the core service methodology behind every Quibble Security compliance engagement. It's designed to be **platform-agnostic** (works whether the client uses Vanta, Drata, OneTrust, AuditBoard, or nothing at all) and **framework-agnostic** (the phases are the same whether the target is SOC 2, HIPAA, NIST CSF, or GLBA Safeguards Rule — only the control set changes).

## Phase 1 — Gap Assessment

**Goal:** Establish an honest, evidence-based baseline of the client's current control environment against the target framework.

**Inputs:**
- Kickoff questionnaire (scoping, systems inventory, prior audit history)
- Stakeholder interviews (IT/engineering lead, HR, leadership)
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

## Phase 4 — Tailored Policy Suite

**Goal:** Deliver a policy set that's actually mapped to the target framework's control requirements and reflects how the client really operates — not generic boilerplate.

**Outputs:**
- Core policy set ([templates](../templates/policy-suite/)): Information Security Policy, Acceptable Use Policy, Incident Response Policy, plus framework-specific additions as needed
- Each policy cross-referenced to the control(s) it satisfies in the control matrix

## How the phases connect

```
Gap Assessment  →  Remediation Roadmap  →  Awareness Training  +  Policy Suite
   (baseline)          (the plan)              (ongoing operational controls)
```

Phases 3 and 4 typically run in parallel once the roadmap is approved. For clients using continuous-monitoring platforms (Vanta, Drata), evidence collected in Phases 3–4 is wired into automated control monitoring — see [compliance-as-code-toolkit](../../compliance-as-code-toolkit) for the automation patterns used to validate and monitor that evidence.
