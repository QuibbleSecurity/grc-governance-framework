# Gap Assessment — IT / Systems Questionnaire

**Client:** [Client Name]
**Prepared by:** Quibble Security LLC

---

**Instructions**

This questionnaire is part of Quibble Security LLC's Gap Assessment for [Client Name]. As the technical lead (CTO / IT Manager / Security Administrator), your responses will help us evaluate [Client Name]'s technical security controls, infrastructure posture, and systems management practices against the target framework's control requirements.

Please be as specific and accurate as possible. If a control is partially in place, describe what exists. If a question does not apply, write "N/A." If you are unsure, write "Unknown" — this is valuable information.

Please return this completed questionnaire to [contact email] within 7 business days. A follow-up call will be scheduled to discuss your responses in detail.

**Respondent Information**

| Field | Response |
|---|---|
| Full Name | |
| Title / Role | |
| Date Completed | |
| Email | |

## Section A — Infrastructure & Cloud Environment

1. **Describe [Client Name]'s current technology infrastructure and cloud environment.** _(e.g., Google Workspace, AWS, GCP, Azure, on-premise servers, SaaS platforms in use)_

2. **What are the primary systems and applications [Client Name] uses to run its business?** _(List key tools: collaboration, CRM, data storage, financial systems, development tools, etc.)_

3. **Are [Client Name]'s systems and data primarily hosted in the cloud? If hybrid (cloud + on-premise), please describe the split.**
   ☐ Yes  ☐ No  ☐ In Progress  ☐ Unknown
   Notes / Details:

4. **Who is responsible for managing and maintaining [Client Name]'s infrastructure? Is this internal staff, a managed service provider, or both?**

## Section B — Access Controls & Identity Management

5. **Is multi-factor authentication (MFA) enforced across all systems and user accounts?** _(Including email/collaboration suite, cloud platforms, admin accounts, and any SaaS tools)_
   ☐ Yes  ☐ No  ☐ In Progress  ☐ Unknown
   Notes / Details:

6. **Does [Client Name] use role-based access control (RBAC) to limit what each user can access?** _(Are permissions assigned based on job function rather than given broadly?)_
   ☐ Yes  ☐ No  ☐ In Progress  ☐ Unknown
   Notes / Details:

7. **How are user accounts and access privileges managed? Who approves and provisions new access?**

8. **Are administrator or privileged accounts limited to only those who require them?** _(e.g., workspace super-admin, cloud root/admin accounts)_
   ☐ Yes  ☐ No  ☐ In Progress  ☐ Unknown
   Notes / Details:

9. **Are there documented password requirements or password policies in place? Please describe.** _(e.g., minimum length, complexity requirements, expiration, use of a password manager)_

10. **Is there a formal process for revoking access when an employee leaves or changes roles?** _(Offboarding checklist, automated de-provisioning, or manual process?)_
    ☐ Yes  ☐ No  ☐ In Progress  ☐ Unknown
    Notes / Details:

## Section C — Endpoint Security & Device Management

11. **Are employee devices company-owned, personally-owned (BYOD), or a mix of both?** _(If BYOD, are there any security requirements employees must meet to use personal devices for work?)_

12. **Is endpoint protection software (antivirus / EDR) installed on employee devices?** _(e.g., CrowdStrike, SentinelOne, Malwarebytes, built-in OS protection)_
    ☐ Yes  ☐ No  ☐ In Progress  ☐ Unknown
    Notes / Details:

13. **Is full-disk encryption enabled on employee laptops and devices?** _(e.g., FileVault on Mac, BitLocker on Windows)_
    ☐ Yes  ☐ No  ☐ In Progress  ☐ Unknown
    Notes / Details:

14. **Does [Client Name] use a Mobile Device Management (MDM) solution?** _(e.g., Jamf, Intune, JumpCloud, Google MDM — used to enforce policies and remotely wipe lost/stolen devices)_
    ☐ Yes  ☐ No  ☐ In Progress  ☐ Unknown
    Notes / Details:

15. **What is [Client Name]'s process if an employee device is lost or stolen? Is remote wipe available?**

## Section D — Logging, Monitoring & Incident Response

16. **Is audit logging enabled across key systems?** _(e.g., workspace admin audit logs, cloud infrastructure logs, application logs)_
    ☐ Yes  ☐ No  ☐ In Progress  ☐ Unknown
    Notes / Details:

17. **Does [Client Name] actively monitor logs or alerts for suspicious activity?** _(e.g., failed logins, privilege escalations, unusual data access)_
    ☐ Yes  ☐ No  ☐ In Progress  ☐ Unknown
    Notes / Details:

18. **Does [Client Name] have a documented incident response plan?** _(A written procedure for how to detect, respond to, and recover from a security incident or data breach)_
    ☐ Yes  ☐ No  ☐ In Progress  ☐ Unknown
    Notes / Details:

19. **Has [Client Name] experienced any security incidents, unauthorized access, or suspected breaches in the past two years? If so, please describe briefly.** _(This information is confidential and used solely for assessment purposes.)_

20. **Who is responsible for responding to security alerts or incidents at [Client Name]? Is there an on-call or escalation process?**

## Section E — Change Management & Vulnerability Management

21. **Does [Client Name] have a formal change management process for updates to systems or infrastructure?** _(e.g., changes are reviewed and approved before deployment, not made ad hoc)_
    ☐ Yes  ☐ No  ☐ In Progress  ☐ Unknown
    Notes / Details:

22. **How are software updates, patches, and security fixes applied across [Client Name]'s systems? How frequently?**

23. **Does [Client Name] conduct vulnerability scans or penetration testing?** _(Automated scans or third-party testing to identify security weaknesses)_
    ☐ Yes  ☐ No  ☐ In Progress  ☐ Unknown
    Notes / Details:

24. **Is there a process for tracking and remediating identified vulnerabilities?** _(e.g., a ticketing system, prioritization framework, or SLA for patching)_
    ☐ Yes  ☐ No  ☐ In Progress  ☐ Unknown
    Notes / Details:

## Section F — Backup, Recovery & Business Continuity

25. **Does [Client Name] have a data backup process in place? Are backups automated, and how frequently are they performed?**
    ☐ Yes  ☐ No  ☐ In Progress  ☐ Unknown
    Notes / Details:

26. **Where are backups stored, and are they stored separately from primary systems (offsite or cloud-based)?**

27. **Has [Client Name] tested its ability to restore data from backups? When was the last restore test conducted?**
    ☐ Yes  ☐ No  ☐ In Progress  ☐ Unknown
    Notes / Details:

28. **Does [Client Name] have a documented Business Continuity or Disaster Recovery plan?** _(A plan for maintaining operations or recovering quickly in the event of a major outage or incident)_
    ☐ Yes  ☐ No  ☐ In Progress  ☐ Unknown
    Notes / Details:

## Section G — Collaboration Suite Security Controls

_(Scope this section to whichever core collaboration platform the client uses — Google Workspace, Microsoft 365, etc.)_

29. **Is MFA enforced at the admin level (not just optional for users)?**
    ☐ Yes  ☐ No  ☐ In Progress  ☐ Unknown
    Notes / Details:

30. **Are file-sharing settings configured to prevent external or "anyone with a link" sharing by default?**
    ☐ Yes  ☐ No  ☐ In Progress  ☐ Unknown
    Notes / Details:

31. **Are admin audit logs enabled and reviewed?** _(Logs covering admin activity, login activity, file-sharing activity, etc.)_
    ☐ Yes  ☐ No  ☐ In Progress  ☐ Unknown
    Notes / Details:

32. **How many users have super-admin privileges? Please list roles if possible.**

33. **Are there any third-party apps or integrations connected to the collaboration suite? Are these reviewed and approved?** _(e.g., OAuth apps, marketplace integrations, connected SaaS tools)_
    ☐ Yes  ☐ No  ☐ In Progress  ☐ Unknown
    Notes / Details:

## Section H — Additional Information

34. **Are there any known security gaps, technical debt, or areas of concern you believe Quibble Security should be aware of?**

35. **Is there anything else about [Client Name]'s technical environment or security posture that is important for this assessment?**

---

*Thank you for completing this questionnaire. Your responses will be used to evaluate [Client Name]'s technical security controls against the target framework's Trust Services Criteria and to develop a prioritized Gap Assessment Report. A follow-up call will be scheduled to discuss your answers in detail.*

