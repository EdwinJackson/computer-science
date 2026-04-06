---
id: FNp4-RgPvfC76pJKjX56atitle: "Security incident handling"
tags:
  - concept
  - knowledge-base
created: 2026-04-06source-count: 7---

# Security incident handling
> [!abstract] About this note
> Conceptual framework synthesised from **7 sources**.
> Expand each section to deepen the framework.

---

## Definition & Scope

> *What is this concept, and what does it include or exclude?*

- Lead efforts to design and collect security operations metrics, and improve the efficiency and effectiveness of incident response plans
- Tackle complex technical issues and problems that cross other teams and significantly impact the business, especially those that other engineers have been unsuccessful in resolving
- Direct the implementation of solutions in collaboration with the team and provide guidance where necessary
- Develop strong relationships with Managers, who help guide rather than direct staff engineers
- Make critical decisions during incidents, including containment actions, ensuring a timely and effective response
- Build and maintain cross-functional relationships with other Staff Engineers and Managers, acting as an extension of leadership and fostering collaboration
- Evangelize best practices, promote security awareness, and drive continuous improvement within the organization
> [!cite]- Primary source
> [Manager, Security Incident...](https://handbook.gitlab.com/job-description-library/security/security-incident-response-team/) · *Mar 11, 2026*
---

## Key Perspectives

> *How do different sources frame this concept?*

### Incident Response SANS: The 6 Steps in Depth - Cynet
- **Setting up monitoring** for all sensitive IT systems and infrastructure.
- **Analyzing events** from multiple sources including log files, error messages, and alerts from security tools.
- **Identifying an incident** by correlating data from multiple sources, and reporting it as soon as possible.
- **Notifying CSIRT members** and establishing communication with a designated command center (for example this could be senior management, IT operations)
> [!cite]- Source · *Mar 19, 2026*> [Incident Response SANS: The 6 Steps in Depth - Cynet](https://www.cynet.com/incident-response/incident-response-sans-the-6-steps-in-depth/)

### SANS Incident Response: 6-Step Process &amp; Critical Best Practices
### Step 1: Preparation
The first step in the SANS Incident Response process involves setting up the right tools, policies, and procedures ahead of any incident, ensuring that the response team can act quickly and efficiently.
This phase includes training staff, creating incident response protocols, and establishing communication strategies both internally and externally.
Organizations must also focus on robust documentation during this stage.
This means gathering and storing reliable contact information for key personnel, delineating clear roles and responsibilities, and ensuring all team members have access to necessary resources.
Being well-prepared reduces chaos and enables more controlled management of incidents.
> [!cite]- Source · *Jul 16, 2025*> [SANS Incident Response: 6-Step Process &amp; Critical Best Practices](https://www.exabeam.com/explainers/incident-response/sans-incident-response-6-step-process-critical-best-practices/)

### Runbook Example: A Best Practices Guide - Nobl9
1. **Level 1 support:** Attempt resolution using the runbook.
2. **Escalate to level 2 support:** Escalate if unresolved within 15 minutes or if the issue exceeds level 1 expertise.
3. **Notify incident manager:** Notify for critical issues that impact service availability or require immediate attention, if more coordination is required.
> [!cite]- Source> [Runbook Example: A Best Practices Guide - Nobl9](https://www.nobl9.com/it-incident-management/runbook-example)

### Security Engineering Manager
- **Monitor and Enforce Security Policies: ** Oversee adherence to IT security policies and controls, partnering with Global Security to ensure enterprise-wide compliance and alignment.
- **Manage Incident Response Procedures: ** Maintain and execute the ADUSA Incident Response Plan across various threat scenarios, including documentation, escalation, and assurance activities.
- **Threat Tracking and Investigation: ** Continuously monitor threat intelligence feeds, analyze alerts from SOC and SIEM systems, and coordinate cross-functional investigations with Group Security, IT, and business stakeholders.
- **First-Line Incident Response: ** Act as the first point of contact for potential security incidents, triaging alerts, initiating response protocols, and ensuring timely communication with IT and Group Security leadership.
- **Security Operations Engagement:** Coordinate with Security Operations Center (SOC) and Group Security threat detection to ensure effective threat monitoring, alert tuning, and response workflows.
> [!cite]- Source · *Nov 2, 2025*> [Security Engineering Manager](https://builtin.com/job/security-engineering-manager/7304565)

### Incident Response Steps &amp; Phases: NIST Framework Explained
- - Endpoint Detection and Response (EDR) or Extended Detection and Response (XDR) solutions.
- Security Information and Event Management (SIEM) systems.
- Network traffic analysis tools.
- Log management and collection systems.
- Intrusion detection and forensic tools.
- **Establish communication protocols and escalation paths.** These workflows should specify who gets contacted at each severity level, preferred communication channels, and approval chains for public statements or regulatory notifications.
…
### Phase 3: Containment, Eradication &amp; Recovery
This phase focuses on stopping the spread of an incident, removing the threat from affected environments, and restoring normal operations.
Although NIST groups containment, eradication, and recovery into one phase, they involve distinct but interconnected actions that occur in parallel.
…
- **Short-term containment:** Immediate steps to stop the attacker’s progress and prevent the spread of the threat.
This may involve isolating affected hosts, cutting off network access, or blocking malicious traffic.
While these actions may cause temporary disruption, they are critical for halting active compromise.
- **Long-term containment:** Measures that maintain limited operations while remediation continues.
These can include segmenting networks, using temporary workarounds to keep critical services available, or shifting workloads to backup systems.
During this phase, systems are hardened and patched to prevent re-entry through the same vulnerabilities.
> [!cite]- Source · *Oct 21, 2025*> [Incident Response Steps &amp; Phases: NIST Framework Explained](https://www.sentinelone.com/cybersecurity-101/services/incident-response-steps-phases/)

### Security Incident Communications Plan - The GitLab Handbook
### Roles and responsibilities in a Security incident
#### Security team roles and responsibilities
|Role|Responsibilities|
|--|--|
|**Security Engineer on Call (SEOC):**|This is the on-call Security Operations Engineer.
The individual is the first to act, validate, and begin the process of determining severity and scope.|
|**Security Incident Manager on Call (SIMOC):**|This is a Security Engineering Manager who is engaged when incident resolution requires coordination across multiple parties.
The SIMOC is the tactical leader of the incident response team, typically not engaged to perform technical work.
The SIMOC assembles the incident team by engaging individuals with the skills, access, and information required to resolve the incident.
The focus of the SIMOC is to keep the incident moving towards resolution, keeping stakeholders informed and performing SecCMOC duties.|
> [!cite]- Source · *Dec 14, 2025*> [Security Incident Communications Plan - The GitLab Handbook](https://handbook.gitlab.com/handbook/security/security-operations/sirt/security-incident-communication-plan/)


---

## Conceptual Map

> *How does **Security incident handling** relate to adjacent concepts?*
> Replace the placeholders with `[[wikilinks]]` to other notes.

| Relation         | Concepts |
| ---------------- | -------- |
| Is a type of     |          |
| Contrasts with   |          |
| Depends on       |          |
| Enables          |          |
| Often confused with |       |

```dataview
LIST
FROM [[Security incident handling]]
SORT file.mtime DESC
```

---

## Applications & Examples

> *Real-world instances, case studies, or demonstrations.*

-

---

## Assumptions & Limitations

> *What does this concept take for granted? Where does it break down?*

-

---

## Open Questions

> *Gaps, tensions, or threads worth investigating further.*

- [ ]

---

## References

1. [Manager, Security Incident...](https://handbook.gitlab.com/job-description-library/security/security-incident-response-team/) *(updated Apr 3, 2026)*2. [Incident Response SANS: The 6 Steps in Depth - Cynet](https://www.cynet.com/incident-response/incident-response-sans-the-6-steps-in-depth/) *(updated Apr 2, 2026)*3. [SANS Incident Response: 6-Step Process &amp; Critical Best Practices](https://www.exabeam.com/explainers/incident-response/sans-incident-response-6-step-process-critical-best-practices/) *(updated Apr 6, 2026)*4. [Runbook Example: A Best Practices Guide - Nobl9](https://www.nobl9.com/it-incident-management/runbook-example) *(updated Apr 4, 2026)*5. [Security Engineering Manager](https://builtin.com/job/security-engineering-manager/7304565) *(updated Oct 4, 2025)*6. [Incident Response Steps &amp; Phases: NIST Framework Explained](https://www.sentinelone.com/cybersecurity-101/services/incident-response-steps-phases/) *(updated Mar 31, 2026)*7. [Security Incident Communications Plan - The GitLab Handbook](https://handbook.gitlab.com/handbook/security/security-operations/sirt/security-incident-communication-plan/) *(updated Mar 28, 2026)*