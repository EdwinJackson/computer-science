---
id: 2fHcb1dAnf34APCAAlwnRtitle: "Service Recovery"
tags:
  - concept
  - knowledge-base
created: 2026-04-06source-count: 12---

# Service Recovery
> [!abstract] About this note
> Conceptual framework synthesised from **12 sources**.
> Expand each section to deepen the framework.

---

## Definition & Scope

> *What is this concept, and what does it include or exclude?*

compromised third-party services to the extent possible.
Recovery progress and resolutions 
are tracked and monitored, and updates are provided to management regularly.
Organisations are responsible for their relationships with their third-party service providers 
and they establish SLAs that include prioritisation of service recovery plans, monitoring 
capabilities, and CIRR reporting in the event that the service provider cannot provide the
> [!cite]- Primary source
> [[PDF] Effective Practices for Cyber Incident Response and Recovery](https://www.fsb.org/uploads/P191020-1.pdf)
---

## Key Perspectives

> *How do different sources frame this concept?*

### Incident Management for Engineering Managers: A Complete Guide
## Your Role During an Incident
During an active incident, the engineering manager&#39;s role is coordination, not execution.
You are not the person debugging the failing service or writing the hotfix - your engineers are.
Your job is to ensure the right people are engaged, communication is flowing to stakeholders, and the team has everything they need to resolve the issue.
…
## Key Takeaways
- Your role during incidents is coordination and communication, not debugging
- Build incident readiness through runbooks, on-call rotations, and regular simulations
- Run blameless post-incident reviews and track action items to completion
- Celebrate reliability wins to build a proactive reliability culture
- Invest in incident management tooling and processes before a major outage forces you to
> [!cite]- Source · *Mar 5, 2026*> [Incident Management for Engineering Managers: A Complete Guide](https://www.em-tools.io/engineering-manager-responsibilities/incident-management)

### What is service recovery? 6 strategies and steps for success - Zendesk
## Service recovery strategies and steps
Here are key strategies and steps in the service recovery process.
1. Get leadership buy-in
2. Establish recovery criteria
3. Create your service recovery team
4. Determine protocol
5. Re-survey the customer
6. Measure impact over time
…
### 3.
Create your service recovery team
Once you’ve established your criteria, it’s important to decide who will be responsible for acting on service recovery tickets.
This decision will be informed by the specifics of your chosen service recovery threshold.
If you’ve set your service recovery for one or two-star interactions, you can assign all service recovery tickets to team leaders.
Alternatively, if you want to tackle all ratings under five stars, you may want to create a team entirely dedicated to service recovery.
In some cases, it might make sense for the agents to handle the service recovery themselves.
It all depends on your team size, overall objectives, and ticket volume.
> [!cite]- Source · *Oct 16, 2019*> [What is service recovery? 6 strategies and steps for success - Zendesk](https://www.zendesk.co.uk/blog/6-steps-build-service-recovery-program/)

### How to Manage Incidents as an Engineering Manager - EM Tools
## Establishing an Incident Response Framework
An incident response framework provides structure during the chaos of a production outage.
Define severity levels with clear criteria - what constitutes a SEV1 versus a SEV3?
Define roles: incident commander (coordinates the response), technical lead (drives diagnosis and resolution), and communications lead (manages stakeholder updates).
These roles should be clearly assigned within the first few minutes of an incident.
…
## Leading During Active Incidents
During an active incident, your primary role as the engineering manager is to ensure the response is coordinated, resources are available, and communication is flowing.
Resist the temptation to take over the technical investigation - your engineers are better positioned for this.
Instead, focus on enabling them to work effectively.
Establish a single communication channel for the incident response team and a separate channel for stakeholder updates.
Mixing operational discussion with stakeholder communication creates confusion and slows both.
Update stakeholders on a regular cadence - every 30 minutes for high-severity incidents - even if the update is &#39;still investigating.&#39;
> [!cite]- Source · *Mar 5, 2026*> [How to Manage Incidents as an Engineering Manager - EM Tools](https://www.em-tools.io/managing-teams/managing-incidents)

### Postmortem Practices for Incident Management - Google SRE
###### Postmortem checklist
To help authors ensure a postmortem is properly completed, we provide a postmortem checklist that walks the owner through key steps.
Here are just a few example checks on the list:
- Perform a complete assessment of incident impact.
- Conduct sufficiently detailed root-cause analysis to drive action item planning.
- Ensure action items are vetted and approved by the technical leads of the service.
- Share the postmortem with the wider organization.
> [!cite]- Source> [Postmortem Practices for Incident Management - Google SRE](https://sre.google/workbook/postmortem-culture/)

### Engineering Manager (Site Reliability) - Rightmove | Built In London
**Incident Management**
- Consistency and standardisation of incident management resulting fast incident detection and resolution
- Maintaining a culture of accountability, transparency, collaboration &amp; learning
- Good data quality, insights &amp; decision‑making with strong feedback loops to all relevant stakeholders
**Reliability Engineering**
- Clear reliability patterns and standards drive strong reliability and fewer cascading failures.
E.g. probes, graceful termination/degradation, timeouts, retries, backoff, jitter, circuit breakers, bulkheads.
- Shared understanding how our system fails, where any weak points are with prioritised improvement plans in place.
> [!cite]- Source> [Engineering Manager (Site Reliability) - Rightmove | Built In London](https://builtinlondon.uk/job/engineering-manager-site-reliability/8624171)

### Post-incident review best practices | Jira Service Management Cloud
### Review every post-incident review
An unreviewed post-incident review might as well not have been written.
Once a post-incident review has been drafted, it’s important to review it to close out any unresolved work items, capture ideas to consider in the future, and finalize the report.
It’s a good idea to schedule a recurring meeting with engineering (and anyone else who may have an interest, like customer support or account managers), at least monthly, to review your post-incident reviews.
You can choose to look over recent reviews or older reports and share any relevant lessons.
…
### 1. Decide which incidents need review
Incidents in your organization should have clear and measurable severity levels.
These severity levels can be used to trigger the post-incident review process.
For example, any incident Sev-1 or higher triggers a post-incident review, while post-incident reviews can be optional for less severe incidents.
Consider allowing team leads or management the opportunity to request a post-incident review for any incident they feel warrants it.
### 2.
Draft your review within two days of the incident
It’s important to take a break and get some rest after an incident.
But don’t delay writing the post-incident review.
Wait too long and important details might be lost or forgotten.
Ideally, it’s drafted immediately after a meeting with the incident team, within 24-48 hours (and not more than five business days) of the incident resolving.
### 3.
Assign roles and owners
Have a meeting to hash out the details that will be recorded into the review.
It’s a good idea to delegate drafting the review to a specific person, ideally someone familiar with the incident who has the required level of technical and organizational knowledge to understand the causes and mitigations.
…
**Important times to include:**
- First alert or ticket
- First comms announcement (internal and/or external)
- Times of status page updates
- Time of any remediation attempts (code rollbacks, etc.)
- Time of resolution
### 6.
Add as many details as possible
Leaving out details is a quick path to writing post-incident reviews that are unhelpful and unclear.
Add as many details as possible about what happened and what was done during the incident.
Instead of “then public comms went out,” say “We sent the initial public comms announcing the incident on our public status page and Twitter account.”
Include as many links as possible to work items, status updates, documentation and monitoring charts, and don’t be afraid to attach relevant screenshots.
> [!cite]- Source · *Nov 29, 2021*> [Post-incident review best practices | Jira Service Management Cloud](https://support.atlassian.com/jira-service-management-cloud/docs/post-incident-review-best-practices/)

### Best Practices for Major Incident Response
focus on service restoration.
• Results in REDUCED TIME TO RESTORE!
• Maintain high availability of technology services critical to 
the business.
• Ensures adherence to First American IT Service 
Management policies &amp; procedures and ITIL best practice 
guidelines.
• Detailed documentation enables accurate reporting and 
facilitate problem reviews to mitigate future recurrences, 
develop preventative strategies and long term remediation 
plan.
Continual Service Improvement (CSI)
Service Recovery Management C.S.I.
Initiative:
•
The Service Recovery Management team conducts ongoing process performance 
assessment through customer surveys and internal process performance evaluation 
exercises.
Post Incident:
•
Customer Surveys for priority 1 incidents and select priority 2s
•
Internal SRM team peer review within 24 Hours of incident resolution
> [!cite]- Source> [Best Practices for Major Incident Response](https://www.thinkhdi.com/~/media/HDIConf/Files/Copy%20of%20Handouts/Session603.pdf)

### Engineering Manager Responsibilities: Complete Guide 2025 - Upstat
## Incident Response and Operational Oversight
### Coordinating Incident Response
Engineering managers play a critical role during production incidents, though not always as hands-on responders:
Ensure clear incident command structure exists and someone takes charge.
When incidents occur without designated leadership, confusion delays resolution.
Your job is making sure an incident commander steps up—whether that’s you, a senior engineer, or whoever’s on-call.
Make resourcing decisions during major incidents.
As incidents escalate, determine whether to pull in additional engineers, wake someone at 3 AM, or let the current on-call handle it.
You balance resolution speed against team sustainability.
Remove blockers preventing responders from doing their work.
Need approval for emergency maintenance window?
Coordinate with leadership.
Need access to external vendor support?
Make those calls.
Your role is clearing the path for technical responders.
> [!cite]- Source · *Oct 26, 2025*> [Engineering Manager Responsibilities: Complete Guide 2025 - Upstat](https://upstat.io/blog/engineering-manager-responsibilities)

### Incident Review: How To Conduct Incident Reviews &amp; Postmortems
#### Key Takeaways
- **Conduct structured, blameless** incident reviews promptly using a consistent agenda and defined roles to identify root causes and ensure accountability.
- **Document incidents thoroughly** and share actionable insights across teams to foster continuous learning and incremental process improvement.
- **Measure the effectiveness of** incident reviews with key metrics like mean time to detect, mean time to resolve, and completion rates for action items to enhance operational resilience.
> [!cite]- Source · *Apr 18, 2024*> [Incident Review: How To Conduct Incident Reviews &amp; Postmortems](https://www.splunk.com/en_us/blog/learn/incident-review-best-practices.html)

### Service Recovery: Definition, Importance &amp; Best Practices
### Develop a solid service recovery plan
Establish a clear protocol for rectifying service failures and ensure all team members clearly understand and adhere to it.
This helps standardize service recovery procedures and ensures that you are consistently professional when dealing with unsatisfied customers.
…
### Find a workable recovery solution
Go beyond a mere apology and focus on finding lasting solutions to the problems that make customers leave.
In the immediate aftermath of an issue, you should set clear expectations for follow-up and resolution timelines.
In the event that a solution isn’t immediately available, let the customer know the steps you will take to find one.
Furthermore, depending on the issue and its scope, you can offer personalized compensation such as discounts, refunds, or a free product or service to make up for the service failure in some way.
> [!cite]- Source · *Jan 1, 2024*> [Service Recovery: Definition, Importance &amp; Best Practices](https://www.bolddesk.com/learn/service-recovery)

### Senior Engineering Manager, Site Reliability
- Embedding SREs in product teams to influence design and early detection of failure modes
- Defining production-readiness checklists and launch gates tied to SLOs
- Championing error budgets as a shared accountability mechanism between product and reliability
- Establish and evolve an incident management practice, including:
- Clear roles (Incident Commander, Scribe, Subject Matter Experts, CX &amp; affected customer communication)
> [!cite]- Source · *Jul 31, 2025*> [Senior Engineering Manager, Site Reliability](https://www.builtinsf.com/job/senior-engineering-manager-site-reliability/6732928)


---

## Conceptual Map

> *How does **Service Recovery** relate to adjacent concepts?*
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
FROM [[Service Recovery]]
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

1. [[PDF] Effective Practices for Cyber Incident Response and Recovery](https://www.fsb.org/uploads/P191020-1.pdf) *(updated Mar 29, 2026)*2. [Incident Management for Engineering Managers: A Complete Guide](https://www.em-tools.io/engineering-manager-responsibilities/incident-management) *(updated Mar 27, 2026)*3. [What is service recovery? 6 strategies and steps for success - Zendesk](https://www.zendesk.co.uk/blog/6-steps-build-service-recovery-program/) *(updated Mar 8, 2026)*4. [How to Manage Incidents as an Engineering Manager - EM Tools](https://www.em-tools.io/managing-teams/managing-incidents) *(updated Mar 22, 2026)*5. [Postmortem Practices for Incident Management - Google SRE](https://sre.google/workbook/postmortem-culture/) *(updated Mar 26, 2026)*6. [Engineering Manager (Site Reliability) - Rightmove | Built In London](https://builtinlondon.uk/job/engineering-manager-site-reliability/8624171) *(updated Mar 6, 2026)*7. [Post-incident review best practices | Jira Service Management Cloud](https://support.atlassian.com/jira-service-management-cloud/docs/post-incident-review-best-practices/) *(updated Mar 30, 2026)*8. [Best Practices for Major Incident Response](https://www.thinkhdi.com/~/media/HDIConf/Files/Copy%20of%20Handouts/Session603.pdf) *(updated Sep 11, 2025)*9. [Engineering Manager Responsibilities: Complete Guide 2025 - Upstat](https://upstat.io/blog/engineering-manager-responsibilities) *(updated Mar 31, 2026)*10. [Incident Review: How To Conduct Incident Reviews &amp; Postmortems](https://www.splunk.com/en_us/blog/learn/incident-review-best-practices.html) *(updated Apr 4, 2026)*11. [Service Recovery: Definition, Importance &amp; Best Practices](https://www.bolddesk.com/learn/service-recovery) *(updated Mar 24, 2026)*12. [Senior Engineering Manager, Site Reliability](https://www.builtinsf.com/job/senior-engineering-manager-site-reliability/6732928) *(updated Aug 7, 2025)*