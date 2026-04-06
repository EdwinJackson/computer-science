---
id: Xaeb67Nqdi0kwvehQUYeJtitle: "Emergency protocols"
tags:
  - concept
  - knowledge-base
created: 2026-04-06source-count: 11---

# Emergency protocols
> [!abstract] About this note
> Conceptual framework synthesised from **11 sources**.
> Expand each section to deepen the framework.

---

## Definition & Scope

> *What is this concept, and what does it include or exclude?*

1 
Incident Response Plan Template 
This document describes the plan for responding to information security incidents at the 
[AGENCY NAME].
It defines the roles and responsibilities of participants, characterization of 
incidents, relationships to other policies and procedures, and reporting requirements.
The goal 
of this any subcontractor Incident Response Plan is to detect and react to computer and
…
iii.
How the incident occurred (email, firewall, etc.) 
iv. Where the attack came from (IP address, physical address, other related 
info) 
v. What the response plan was. 
vi.
What was done in response. 
vii.
Whether the response was effective. 
viii.
Recommendations for procedure improvement.
> [!cite]- Primary source
> [[PDF] Incident Response Plan Template](https://primacentral.org/wp-content/uploads/2023/05/Incident-Response-Plan-Template.pdf)
---

## Key Perspectives

> *How do different sources frame this concept?*

### IT Disaster Recovery Crisis Communications - Template
Create a process that describes under what conditions a Crisis Communications Plan is to be activated.
It should contain what the 
process is and who is authorized to activate the plan.
Notification Process 
Activity 4 – Notification Process  
1. 
Document how Executive and Management teams, recovery teams, staff, vendors, stakeholders, etc, will be notified.
…
cell towers are impacted by a natural disaster, etc.
2. 
Develop contingency plans for each scenario.
3. 
Create assessment procedures.
Determine how ‘on the scene’ information will be provided to the Crisis Communications team 
and by whom.
Note: Consult with the Business Continuity Officer.
Messaging 
Activity 7 – Key Messages 
During a crisis, it may be helpful to have pre-canned key messages already developed.
Messages should be created for different 
types and scopes of outages and disasters.
This will save time when delivering notifications to Executives, stakeholders, 
employees, vendors, etc.
> [!cite]- Source> [IT Disaster Recovery Crisis Communications - Template](https://cyberalberta.ca/system/files/it-disaster-recovery-crisis-communications-framework-template.pdf)

### A manager&#39;s guide to improving on-call - Atlassian
- **De-duplicating related alerts** to avoid alert fatigue.
- **Designing rich alerts** that clearly describe an issue and empower the on-call engineers to make effective decisions and apply the knowledge recorded in runbooks.
- **Providing alert reports and metrics ** to on-call teams so that weak areas in systems can be identified and improved.
(In other words: don’t let on-call teams get bogged down by the same issues over and over again.)
> [!cite]- Source · *Dec 9, 2025*> [A manager&#39;s guide to improving on-call - Atlassian](https://www.atlassian.com/incident-management/on-call/improving-on-call)

### How To Make an Incident Response Plan (Template ...
- Detail which systems and infrastructure are covered by the incident response plan.
- For planning purposes, consider defining an “incident” to be any confirmed or suspected unauthorized access to, or misuse of, your information systems, data or facilities.
- Specify who has authority to execute the plan, such as which stakeholders from IT, legal, HR, management, etc., are involved in the response activities.
…
- **Identification **– How will you monitor alerts from security tools, employee reports and customer complaints?
Describe how you will assess severity and document what happened, when it was discovered, systems affected and potential impact.
- **Containment **– What immediate actions will your team take to stop the incident from spreading?
What measures will be implemented to maintain your business operations while addressing the incident?
> [!cite]- Source · *Sep 28, 2025*> [How To Make an Incident Response Plan (Template ...](https://warrenaverett.com/insights/incident-response-plan-template-included/)

### On Call Engineer Best Practices for IT Services - Google SRE
When one is handling incidents, if the issue is complex enough to involve multiple teams or if, after some investigation, it is not yet possible to estimate an upper bound for the incident’s time span, it can be useful to adopt a formal incident-management protocol.
Google SRE uses the protocol described in Managing Incidents, which offers an easy-to-follow and well-defined set of steps that aid an on-call engineer to rationally pursue a satisfactory incident resolution with all the required help.
> [!cite]- Source> [On Call Engineer Best Practices for IT Services - Google SRE](https://sre.google/sre-book/being-on-call/)

### Incident response plan templates | Red Canary
## Incident response template examples
### NIST Incident Response Plan
The NIST Special Publication 800 NIST SP 800-61r3, titled “Incident Response Recommendations and Considerations for Cybersecurity Risk Management” provides a comprehensive framework and guidelines for organizations to establish and maintain robust incident response capabilities.
It outlines a structured incident response lifecycle framed through NIST’s Cybersecurity Framework (CSF) 2.0’s six core functions, including govern, identify, protect, detect, respond, and recover.
The publication—and its predecessor NIST Special Publication 800-61, Revision 2, Computer Security Incident Handling Guide—have served as globally recognized standards for effective incident management.
…
**Form an incident response team (IRT)**
Assemble a dedicated team with diverse skill sets, including technical experts, legal counsel, communications specialists, and management representatives.
Clearly define each member’s specific roles and responsibilities within the response framework.
**Establish training and awareness programs**
Regularly train IRT members on incident handling procedures, tools, and technologies.
Conduct organization-wide security awareness training to educate employees on recognizing and reporting suspicious activities, fostering a security-conscious culture.
…
**Establish robust alerting mechanisms**
Configure automated alerts for suspicious activities or predefined security thresholds, ensuring that the IRT is promptly notified of potential incidents.
Prioritize alerts based on severity and potential impact.
**Perform initial assessment and triage**
Quickly determine the scope, severity, and potential impact of a detected event.
This involves categorizing the incident, assessing the systems affected, and estimating the potential data compromised.
> [!cite]- Source · *Jul 23, 2025*> [Incident response plan templates | Red Canary](https://redcanary.com/cybersecurity-101/incident-response/incident-response-plan-template/)

### Best Practices For Building A Resilient On-Call Framework
## Best Practices For An Effective On Call Framework
- Define transparent roles and responsibilities for On-Call Members
- Clear handling procedure with rotation strategy
- Incident classification &amp; prioritization
- Implement role based control within organization
- Document results &amp; learn from past incidents
- Proactive collaboration during incident resolution
- Scheduling for unavailability
- On Call Management Tool
…
- avoid wasting time on low-priority issues
- focus their efforts on resolving high-impact incidents first
- minimizing downtime and maintain service levels
- respond more quickly and appropriately
- minimize the overall time to resolution (TTOR) for all incidents
- make informed decisions
On top of this tracking key metrics like response times, resolution times, and escalation rates can help identify areas for improvement.
### 4.
Implement Role Based Access Control
Implementing Role-Based Access Control (RBAC) in an On-Call framework helps in two key ways:
- Firstly, it ensures only authorized personnel can have access to On-Call tools and monitoring systems based on their roles and responsibilities.
It minimizes the risk of unauthorized access, accidental changes, or data breaches that could disrupt operations or compromise sensitive information.
- Secondly, it also streamlines workflows by granting appropriate permissions to different roles.
This allows on-call personnel to focus on their specific tasks without getting overwhelmed by unnecessary information or functionalities, leading to faster incident resolution and improved overall efficiency.
### 5.
Document results &amp; learn from past incidents
Analyzing past incident reports helps identify recurring patterns and underlying root causes.
This allows teams to address systemic issues and prevent similar incidents from happening again, leading to a more proactive and preventative approach to Incident Management.
Documenting postmortem analysis findings, including lessons learned and action items, provides a structured roadmap for continuous improvement.
This allows teams to identify weaknesses in the** On-Call framework, implement corrective measures, and refine best practices for handling future incidents.** Additionally, On-Call teams can establish baselines for key metrics and make data-driven decisions.
> [!cite]- Source> [Best Practices For Building A Resilient On-Call Framework](https://www.squadcast.com/blog/best-practices-for-building-a-resilient-on-call-framework)

### How to Create a Crisis Communication Plan - Everbridge
- Pre-defined communication protocols
- Assigned roles and responsibilities
- Key messaging templates for various scenarios
- Internal and external communication workflows
- Multi-channel deployment of critical updates
Whether dealing with a cybersecurity breach, a natural disaster, or a corporate scandal, a well-prepared crisis communication plan acts as the backbone of any response strategy.
> [!cite]- Source · *May 19, 2025*> [How to Create a Crisis Communication Plan - Everbridge](https://www.everbridge.com/blog/crisis-communication-plan/)

### How to Improve On-Call with Better Practices and Tools | FireHydrant
While you *can* manage on-call manually, the right platform can make scheduling, escalation, and incident response far easier and more reliable.
When evaluating on-call tools, look for:
- Multi-channel alerting (phone, SMS, chat, email)
- Broad integrations with your monitoring, logging, and collaboration stack
- Alert grouping, filtering, and de-duplication to cut noise
- Team-based schedule management
- Calendar visualization for quick coverage checks
- Analytics to track workload and coverage gaps
- High delivery reliability for alerts
> [!cite]- Source · *Aug 7, 2024*> [How to Improve On-Call with Better Practices and Tools | FireHydrant](https://firehydrant.com/blog/how-to-improve-on-call-with-better-practices-and-tools/)

### Crisis Communication Plan Template: What to Say (and When ...
|Audience|What They Need|When|Regulatory Driver|
|--|--|--|--|
|**Employees**|Safety instructions, role assignments, status updates|Immediately (within minutes)|OSHA, duty of care|
|**Regulators**|Incident classification, impact assessment, remediation plan|Within 36 hours for qualifying incidents|OCC/FDIC/Fed Computer-Security Incident Notification Rule|
|**Customers**|Service status, workarounds, timeline for restoration|Within 1-4 hours of customer-facing impact|State breach notification laws, UDAP/UDAAP|
…
### Template 4: Business Partner / Vendor Communication (Contractual — Within 4-8 Hours)
**Channel:** Designated contact per vendor/partner agreement
**Timeline:** Per contractual notification requirements (typically 4-24 hours)
**Sent by:** Vendor Management or Third-Party Risk team
Key elements:
- **Which shared systems or data may be affected**
- **Whether the disruption originated in your environment or theirs** (this matters for liability)
- **Actions you need from them** (e.g., “please suspend automated data feeds until further notice”)
- **Reference the specific contract clause** triggering the notification
…
## Building Your Crisis Communication Plan: The 30-Day Implementation Roadmap
### Days 1-7: Foundation
**Owner:** Chief Risk Officer or Head of Compliance
**Deliverables:**
- Identify your four audience groups and map key contacts for each
- Inventory existing notification obligations: regulatory timelines, contractual SLAs, state breach notification laws
- Designate a Communications Lead and backup (this should not be the same person as the Incident Commander)
- Select your mass notification tool — this can’t be “someone sends an email.”
Use a system that can reach employees via SMS, email, and phone simultaneously
…
### Days 15-21: Integration and Testing
**Owner:** Communications Lead + IT + Business Continuity
**Deliverables:**
- Integrate communication templates into your incident response workflow — they should trigger automatically when an incident is classified
- Test the mass notification system (send a test message to all employees)
- Verify regulatory contact information is current — call your OCC/FDIC/Fed examiner’s office and confirm the notification email/portal
- Verify vendor contact lists match current contracts
> [!cite]- Source · *Mar 24, 2026*> [Crisis Communication Plan Template: What to Say (and When ...](https://risktemplate.com/blog/2026-03-25-crisis-communication-plan-template-guide/)

### Pros and cons of different approaches to on-call management
Here are a few tactics to help keep IT incidents manageable:
- **Prompt and transparent communication**: Proactively communicating IT incidents shows you care – and that you&#39;re in control.
- **Keep track of what counts**: Most IT service teams are using some form of service desk software.
It’s critical that you aren’t just using free-form data entry fields to capture the details of each ticket.
- **Put a monitoring system in place**: Historically, many IT Ops teams would personally monitor performance dashboards to keep an eye out for outages.
Do the team a favor and let monitoring and alerting tools handle this.
> [!cite]- Source · *Dec 9, 2025*> [Pros and cons of different approaches to on-call management](https://www.atlassian.com/incident-management/on-call)


---

## Conceptual Map

> *How does **Emergency protocols** relate to adjacent concepts?*
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
FROM [[Emergency protocols]]
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

1. [[PDF] Incident Response Plan Template](https://primacentral.org/wp-content/uploads/2023/05/Incident-Response-Plan-Template.pdf) *(updated Mar 30, 2026)*2. [IT Disaster Recovery Crisis Communications - Template](https://cyberalberta.ca/system/files/it-disaster-recovery-crisis-communications-framework-template.pdf) *(updated Apr 5, 2026)*3. [A manager&#39;s guide to improving on-call - Atlassian](https://www.atlassian.com/incident-management/on-call/improving-on-call) *(updated Mar 26, 2026)*4. [How To Make an Incident Response Plan (Template ...](https://warrenaverett.com/insights/incident-response-plan-template-included/) *(updated Mar 25, 2026)*5. [On Call Engineer Best Practices for IT Services - Google SRE](https://sre.google/sre-book/being-on-call/) *(updated Mar 30, 2026)*6. [Incident response plan templates | Red Canary](https://redcanary.com/cybersecurity-101/incident-response/incident-response-plan-template/) *(updated Mar 31, 2026)*7. [Best Practices For Building A Resilient On-Call Framework](https://www.squadcast.com/blog/best-practices-for-building-a-resilient-on-call-framework) *(updated Apr 6, 2026)*8. [How to Create a Crisis Communication Plan - Everbridge](https://www.everbridge.com/blog/crisis-communication-plan/) *(updated Apr 6, 2026)*9. [How to Improve On-Call with Better Practices and Tools | FireHydrant](https://firehydrant.com/blog/how-to-improve-on-call-with-better-practices-and-tools/) *(updated Apr 6, 2026)*10. [Crisis Communication Plan Template: What to Say (and When ...](https://risktemplate.com/blog/2026-03-25-crisis-communication-plan-template-guide/) *(updated Apr 5, 2026)*11. [Pros and cons of different approaches to on-call management](https://www.atlassian.com/incident-management/on-call) *(updated Apr 1, 2026)*