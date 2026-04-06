---
id: o1xPrfg8iNWQpD12xsbQJtitle: "Incident Management"
tags:
  - concept
  - knowledge-base
created: 2026-04-06source-count: 12---

# Incident Management
> [!abstract] About this note
> Conceptual framework synthesised from **12 sources**.
> Expand each section to deepen the framework.

---

## Definition & Scope

> *What is this concept, and what does it include or exclude?*

## Pick your communication solutions, channels, and message templates ahead of time
Professional support teams and site reliability engineers don’t decide on the fly what channels to communicate over.
They make a plan ahead of time.
There are five main communication channels for incident communication:
- A dedicated status page
- Embedded status
- Email
- Workplace chat tool
- Social media
- SMS
> [!cite]- Primary source
> [Incident communication best practices](https://www.atlassian.com/incident-management/incident-communication) · *Dec 9, 2025*
---

## Key Perspectives

> *How do different sources frame this concept?*

### Post-incident review best practices | Jira Service Management Cloud
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
> [!cite]- Source · *Nov 29, 2021*> [Post-incident review best practices | Jira Service Management Cloud](https://support.atlassian.com/jira-service-management-cloud/docs/post-incident-review-best-practices/)

### Complete Guide to Incident Response for Engineering Teams
### Establishing Communication Channels
Establish dedicated channels for incident coordination before you need them.
Create incident-specific channels with clear naming conventions for each major incident.
Use separate channels for stakeholder notifications to leadership and adjacent teams.
Maintain public status pages for external customer communication.
Set up support coordination channels connecting support teams with technical response.
…
### Following Incident Command Structure
Once declared, assign an Incident Commander who focuses on coordination while technical responders concentrate on fixes.
Establish communication rhythm with regular updates every 15-30 minutes.
Separate investigation from communication so technical responders aren’t context-switching between debugging and stakeholder updates.
Document everything in a clear timeline capturing actions, decisions, and findings.
The Incident Lead should prioritize coordination over hands-on technical work.
Their job is ensuring the right people work on the right things, not implementing fixes themselves.
…
### Three Communication Layers
Effective incident communication operates at three distinct layers, each requiring different messaging, cadence, and channels.
Internal team coordination focuses on investigation and resolution.
Participants need technical details, raw findings, and real-time updates on what’s been tried and what remains.
Use dedicated incident channels that persist after resolution, document findings immediately, keep updates frequent but concise, and maintain running timelines.
> [!cite]- Source · *Oct 25, 2025*> [Complete Guide to Incident Response for Engineering Teams](https://upstat.io/blog/incident-response-guide)

### How to Build Incident Response Playbooks - OneUptime
```
## Incident Roles
### Incident Commander (IC)
- Coordinates overall response
- Makes decisions on escalation and communication
- Tracks timeline and action items
- Does NOT troubleshoot directly
### Technical Lead
- Leads diagnosis and remediation efforts
- Coordinates between multiple engineers if needed
- Provides technical updates to IC
### Communications Lead
- Updates status page
- Handles customer communications
- Notifies stakeholders
- Documents timeline in incident channel
### Scribe (optional for SEV1/SEV2)
- Records all actions taken
- Tracks who did what and when
- Prepares postmortem timeline
```
…
### Internal Communication Templates
```
## Slack Templates
### Incident Declaration
:rotating_light: INCIDENT DECLARED - SEV[X]
Service: [affected service]
Impact: [user-facing impact]
IC: @[name]
Tech Lead: @[name]
War Room: [link to video call]
Status Page: [link]
### Handoff Template
:arrows_counterclockwise: INCIDENT HANDOFF
Outgoing IC: @[name]
Incoming IC: @[name]
Current Status: [brief summary]
Active Actions: [list]
Next Steps: [list]
```
> [!cite]- Source · *Jan 26, 2026*> [How to Build Incident Response Playbooks - OneUptime](https://oneuptime.com/blog/post/2026-01-27-incident-response-playbooks/view)

### Guide to Effective Post-Incident Reviews - OnPage
- **Identify Underlying Causes of the Incident**
Once the post-incident report has been shared, teams can begin to identify the underlying causes of the incident.
Some of the causes may have already been noted in the incident report, but as mentioned previously there is not always one cause to an incident.
This ensures that all potential causes have been exhausted so that engineers can have a clear understanding of which systems may need extra attention.
> [!cite]- Source · *Oct 9, 2025*> [Guide to Effective Post-Incident Reviews - OnPage](https://www.onpage.com/onpage-university/guide-to-post-incident-reviews/)

### Incident Review and Postmortem Best Practices
- **Leave time for engineers to work on an incident review/postmortem**.
While it’s always possible to rush this process, you’ll get lower quality reviews if you do so.
Instead, give people the space to get together and discuss what happened, and aim for all those involved to have their say.
- **Dig deeper when looking into root causes of the incident.** Don’t stop at the first and often obvious, potential reason.
Ask questions to understand how various factors could have contributed to the outage, and what are the things that contributed to those factors.
> [!cite]- Source · *Oct 18, 2021*> [Incident Review and Postmortem Best Practices](https://newsletter.pragmaticengineer.com/p/incident-review-best-practices)

### Learn sre incident management and response - Google SRE
IMAG organizes the incident response by establishing a hierarchical structure with clear roles, tasks, and communication channels.
The main roles in Google&#39;s IMAG are Incident Commander (IC), Communications Lead (CL), and Operations Lead (OL).
The IC coordinates the overall incident response.
The CL provides regular updates to stakeholders and acts as a point of contact for incoming communications.
> [!cite]- Source> [Learn sre incident management and response - Google SRE](https://sre.google/resources/practices-and-processes/incident-management-guide/)

### How to create an incident response playbook - Work Life by Atlassian
**Example:**
As a new incident is detected, the incident manager begins initiating internal communication and response organization.
This the team can begin working on fixing the cause of the incident and reaching a resolution.
Strong organization in this stage facilitates action, which is powered by frequent communication.
Adhering to a consistent process leads to a faster resolution, including a postmortem exercise we will cover below.
> [!cite]- Source · *Apr 15, 2020*> [How to create an incident response playbook - Work Life by Atlassian](https://www.atlassian.com/blog/it-teams/how-to-create-an-incident-response-playbook/amp)

### Incident Review: How To Conduct Incident Reviews &amp; Postmortems
#### Key Takeaways
- **Conduct structured, blameless** incident reviews promptly using a consistent agenda and defined roles to identify root causes and ensure accountability.
- **Document incidents thoroughly** and share actionable insights across teams to foster continuous learning and incremental process improvement.
- **Measure the effectiveness of** incident reviews with key metrics like mean time to detect, mean time to resolve, and completion rates for action items to enhance operational resilience.
> [!cite]- Source · *Apr 18, 2024*> [Incident Review: How To Conduct Incident Reviews &amp; Postmortems](https://www.splunk.com/en_us/blog/learn/incident-review-best-practices.html)

### How to run a major incident management process | Atlassian
### Opening comms
Once the incident manager gets an alert, their first order of business is to communicate that the incident fix is in progress.
They change the status of the incident to fixing and set up the team’s communication channels.
It&#39;s imperative to offer flexible communication channels throughout the incident response process that allow teams to stay in touch by their preferred method.
Jira Service Management integrates multiple communications channels to minimize downtime, such as embeddable status widget, dedicated statuspage, email, chat tools, social media, and SMS.
…
Speedy, accurate communication helps build and keep customer trust.
We have a strategic incident communication plan and provide regular status updates that follow a simple format.
We also send an email to a set list of stakeholders that includes our engineering leadership, major incident managers, and other key internal staff.
As previously mentioned, all of these communication methods are customizable within Jira Service Management and can be tailored to any organization&#39;s incident response plan.
> [!cite]- Source · *Dec 9, 2025*> [How to run a major incident management process | Atlassian](https://www.atlassian.com/incident-management/itsm/major-incident-management)

### What is an Incident Response Playbook? - Palo Alto Networks
### Communication and Coordination Strategy
Effective communication is at the heart of any incident response strategy.
A well-defined communication plan ensures timely updates reach the right people through primary channels like email or secure video conferencing.
Regular status meetings allow team members to report progress and adjust plans as needed.
The plan also outlines protocols for collaborating with external partners, such as cybersecurity experts and law enforcement, to leverage expertise and meet legal obligations.
> [!cite]- Source> [What is an Incident Response Playbook? - Palo Alto Networks](https://www.paloaltonetworks.com/cyberpedia/what-is-an-incident-response-playbook)

### Best practices in post incident reviews dramatically ...
#### Evaluate the use of data and tools for diagnostics
Incident troubleshooting frequently comes down to having the right tools and data available for subject matter experts to use in understanding what is going on and diagnosing underlying issues.
The post-incident review should include a review of what data and tools were available, which were used and what data and tools the team wishes had been available to make the process easier.
Frequently the incident support team is unaware of tools and resources that actually were available.
The PIR can help identify these resources and ensure that staff has access and knows how to use them during the next incident.
> [!cite]- Source · *Jul 9, 2025*> [Best practices in post incident reviews dramatically ...](https://kepner-tregoe.com/blogs/best-practices-in-post-incident-reviews-dramatically-improve-incident-response/)


---

## Conceptual Map

> *How does **Incident Management** relate to adjacent concepts?*
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
FROM [[Incident Management]]
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

1. [Incident communication best practices](https://www.atlassian.com/incident-management/incident-communication) *(updated Apr 5, 2026)*2. [Post-incident review best practices | Jira Service Management Cloud](https://support.atlassian.com/jira-service-management-cloud/docs/post-incident-review-best-practices/) *(updated Mar 30, 2026)*3. [Complete Guide to Incident Response for Engineering Teams](https://upstat.io/blog/incident-response-guide) *(updated Oct 27, 2025)*4. [How to Build Incident Response Playbooks - OneUptime](https://oneuptime.com/blog/post/2026-01-27-incident-response-playbooks/view) *(updated Apr 5, 2026)*5. [Guide to Effective Post-Incident Reviews - OnPage](https://www.onpage.com/onpage-university/guide-to-post-incident-reviews/) *(updated Apr 5, 2026)*6. [Incident Review and Postmortem Best Practices](https://newsletter.pragmaticengineer.com/p/incident-review-best-practices) *(updated Feb 24, 2026)*7. [Learn sre incident management and response - Google SRE](https://sre.google/resources/practices-and-processes/incident-management-guide/) *(updated Apr 6, 2026)*8. [How to create an incident response playbook - Work Life by Atlassian](https://www.atlassian.com/blog/it-teams/how-to-create-an-incident-response-playbook/amp) *(updated Mar 25, 2026)*9. [Incident Review: How To Conduct Incident Reviews &amp; Postmortems](https://www.splunk.com/en_us/blog/learn/incident-review-best-practices.html) *(updated Apr 4, 2026)*10. [How to run a major incident management process | Atlassian](https://www.atlassian.com/incident-management/itsm/major-incident-management) *(updated Apr 5, 2026)*11. [What is an Incident Response Playbook? - Palo Alto Networks](https://www.paloaltonetworks.com/cyberpedia/what-is-an-incident-response-playbook) *(updated Apr 1, 2026)*12. [Best practices in post incident reviews dramatically ...](https://kepner-tregoe.com/blogs/best-practices-in-post-incident-reviews-dramatically-improve-incident-response/) *(updated Nov 11, 2025)*