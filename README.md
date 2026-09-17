# GRC Governance Framework

A platform-agnostic governance, risk, and compliance (GRC) methodology and template library, developed and maintained by **Quibble Security LLC**.

This repository is the public, redacted version of the working methodology and document set used in client engagements — gap assessments, remediation roadmaps, control mappings, and policy suites — generalized so they can be reused across verticals (financial services, healthcare, education, professional services) and mapped to common frameworks (SOC 2, NIST CSF, ISO 27001, HIPAA, PCI-DSS, GLBA Safeguards Rule).

All client names, data, and identifying details in this repository are fictional or fully anonymized. Nothing here reflects a real client's actual environment, findings, or risk posture.

> Looking for the automation side of this work — scripts that validate control mappings, check evidence freshness, and run as CI checks? See [compliance-as-code-toolkit](../compliance-as-code-toolkit).

## Why this exists

Compliance work is often treated as a one-off document exercise. This repository documents a **repeatable, four-phase engagement model** so that gap assessments, remediation plans, and policy suites are consistent, auditable, and reusable across clients and frameworks — rather than rebuilt from scratch every time.

## The Four-Phase Framework

1. **Gap Assessment** — baseline the client's current control environment against the target framework(s); produce a scored gap assessment report.
2. **Remediation Roadmap** — translate gaps into a prioritized, resourced roadmap (technical remediation, policy, training) with owners and target dates.
3. **Security Awareness Training** — role-based training and phishing simulation program, scoped to the client's size and risk profile.
4. **Tailored Policy Suite** — a policy set mapped to the target framework's control requirements, written for the client's actual environment rather than generic boilerplate.

See [`methodology/four-phase-framework.md`](methodology/four-phase-framework.md) for the full write-up of each phase, inputs, outputs, and typical timeline.

## Service offerings

Some parts of the framework are also sold as standalone services, independent of a full four-phase engagement:

- [Security Awareness Training Program](service-offerings/security-awareness-training-program.md) — a 12-month program of tailored live training, quarterly phishing simulations, and audit-ready documentation.

## Repository structure

```
grc-governance-framework/
├── methodology/            # The engagement model itself
│   └── four-phase-framework.md
├── templates/               # Reusable, framework-agnostic document templates
│   ├── gap-assessment-report-template.md
│   ├── remediation-roadmap-template.md
│   ├── control-matrix-template.csv
│   ├── role-based-access-matrix-template.csv
│   ├── questionnaires/       # Phase 1 stakeholder intake questionnaires
│   │   ├── executive-leadership-questionnaire-template.md
│   │   ├── it-systems-questionnaire-template.md
│   │   ├── finance-operations-questionnaire-template.md
│   │   └── people-hr-questionnaire-template.md
│   └── policy-suite/
│       ├── information-security-policy-template.md
│       ├── acceptable-use-policy-template.md
│       ├── incident-response-policy-template.md
│       ├── onboarding-policy-template.md
│       └── offboarding-policy-template.md
├── service-offerings/       # Standalone services, sold independently of the full engagement
│   └── security-awareness-training-program.md
├── case-studies/            # Anonymized, illustrative engagement summaries
│   └── example-soc2-readiness-engagement.md
└── docs/
    └── framework-crosswalk.md   # SOC 2 / NIST CSF / ISO 27001 / HIPAA mapping notes
```

## Frameworks referenced

SOC 2 (Trust Services Criteria), NIST CSF 2.0, ISO/IEC 27001, HIPAA Security Rule, PCI-DSS, GLBA Safeguards Rule, CMMC.

## About

**Quibble Security LLC** is a GRC-focused cybersecurity consultancy specializing in compliance readiness, gap assessments, and remediation program management for small and mid-sized organizations.

- Website: [quibblesecurity.com](https://www.quibblesecurity.com)
- LinkedIn: [mansa-quintyne-ii](https://www.linkedin.com/in/mansa-quintyne-ii-79233b191/)

## License

© 2026 Quibble Security LLC. All rights reserved. This repository is published for reference and portfolio purposes only — see [LICENSE](LICENSE). The methodology, templates, and questionnaires here are illustrative starting points, not a substitute for a tailored engagement, and may not be reproduced, reused, or redistributed without written permission.

