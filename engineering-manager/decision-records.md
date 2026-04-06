---
id: dTjp_rEl1ITZjvELqVtfvtitle: "Decision records"
tags:
  - concept
  - knowledge-base
created: 2026-04-06source-count: 9---

# Decision records
> [!abstract] About this note
> Conceptual framework synthesised from **9 sources**.
> Expand each section to deepen the framework.

---

## Definition & Scope

> *What is this concept, and what does it include or exclude?*

Architecture decision records (ADRs) help you document and communicate important process and architecture decisions in your engineering projects.
Based on our experience implementing over 200 ADRs across multiple projects, we’ve developed best practices that can help you streamline your decision-making processes and improve team collaboration.
…
5. **Separate design from decision** – Use a separate design document mechanism to explore alternative options thoroughly.
Reference these design documents within the ADR, adhering to the principles of invention and simplification.
6. **Address comments and resolve feedback** – Actively follow up on comments received during the ADR review process.
Resolve all comments, either by incorporating changes or by discussing and reaching a consensus with the comment author.
This practice demonstrates a commitment to delivering results and fostering a sense of ownership.
> [!cite]- Primary source
> [Master architecture decision records (ADRs): Best practices ... - AWS](https://aws.amazon.com/blogs/architecture/master-architecture-decision-records-adrs-best-practices-for-effective-decision-making/) · *Mar 19, 2025*
---

## Key Perspectives

> *How do different sources frame this concept?*

### Loqbooq — Free Decision Log for Your Project
## Architectural Decision Records (ADR)
Loqbooq is a lightweight tool for recording technical decisions
in coding or engineering projects.
New members joining your team will find it easier to get their head around your design and architecture when they can look up why things were done how they were done.
> [!cite]- Source> [Loqbooq — Free Decision Log for Your Project](https://loqbooq.app)

### ADR Template | MADR
# {short title, representative of solved problem and found solution}
## Context and Problem Statement
{Describe the context and problem statement, e.g., in free form using two to three sentences or in the form of an illustrative story.
You may want to articulate the problem in form of a question and add links to collaboration boards or issue management systems.}
> [!cite]- Source> [ADR Template | MADR](https://adr.github.io/madr/decisions/adr-template.html)

### 8 best practices for creating architecture decision records | TechTarget
### 5.
Establish clear decision status indicatorss
An effective ADR system should include clear status indicators for each decision.
Common statuses include &quot;Proposed,&quot; &quot;Accepted,&quot; &quot;Deprecated,&quot; and &quot;Superseded.&quot;
Having explicit status markers helps team members understand which architectural decisions are active, under consideration or replaced by newer decisions.
When a decision is superseded, the new ADR should reference the old one and explain why a change was necessary.
…
- **Better collaboration and alignment.** The structured ADR format forces teams to consider alternatives and tradeoffs explicitly, leading to more deliberate decision-making.
- **Accelerated incident resolution.** ADRs provide context for system design choices during production incidents.
- **Reusable resource.** Well-structured ADRs become valuable assets beyond individual projects.
Organizations can mine these records for patterns and reusable solutions, accelerating similar initiatives.
…
### 5.
Establish clear decision status indicatorsrsAn effective ADR system should include clear status indicators for each decision.
Common statuses include &quot;Proposed,&quot; &quot;Accepted,&quot; &quot;Deprecated,&quot; and &quot;Superseded.&quot;
Having explicit status markers helps team members understand which architectural decisions are active, under consideration or replaced by newer decisions.
When a decision is superseded, the new ADR should reference the old one and explain why a change was necessary.
…
> [!cite]- Source · *Jun 19, 2025*> [8 best practices for creating architecture decision records | TechTarget](https://www.techtarget.com/searchapparchitecture/tip/4-best-practices-for-creating-architecture-decision-records)

### About MADR
```
---
# Configuration for the Jekyll template &quot;Just the Docs&quot;
parent: Decisions
nav_order: 100
title: ADR Template
# These are optional elements.
Feel free to remove any of them.
# status: &quot;{proposed | rejected | accepted | deprecated | … | superseded by ADR-0123&quot;
# date: {YYYY-MM-DD when the decision was last updated}
# decision-makers: {list everyone involved in the decision}
# consulted: {list everyone whose opinions are sought (typically subject-matter experts); and with whom there is a two-way communication}
# informed: {list everyone who is kept up-to-date on progress; and with whom there is a one-way communication}
---
&lt;!-- we need to disable MD025, because we use the different heading &quot;ADR Template&quot; in the homepage (see above) than it is foreseen in the template --&gt;
&lt;!-- markdownlint-disable-next-line MD025 --&gt;
# {short title, representative of solved problem and found solution}
## Context and Problem Statement
{Describe the context and problem statement, e.g., in free form using two to three sentences or in the form of an illustrative story.
You may want to articulate the problem in form of a question and add links to collaboration boards or issue management systems.}
&lt;!-- This is an optional element.
Feel free to remove.
--&gt;
## Decision Drivers
* {decision driver 1, e.g., a force, facing concern, …}
* {decision driver 2, e.g., a force, facing concern, …}
* … &lt;!-- numbers of drivers can vary --&gt;
## Considered Options
* {title of option 1}
* {title of option 2}
* {title of option 3}
* … &lt;!-- numbers of options can vary --&gt;
## Decision Outcome
Chosen option: &quot;{title of option 1}&quot;, because {justification.
e.g., only option, which meets k.o. criterion decision driver | which resolves force {force} | … | comes out best (see below)}.
&lt;!-- This is an optional element.
Feel free to remove.
--&gt;
### Consequences
* Good, because {positive consequence, e.g., improvement of one or more desired qualities, …}
* Bad, because {negative consequence, e.g., compromising one or more desired qualities, …}
* … &lt;!-- numbers of consequences can vary --&gt;
&lt;!-- This is an optional element.
Feel free to remove.
--&gt;
### Confirmation
{Describe how the implementation of/compliance with the ADR can/will be confirmed.
Is the chosen design and its implementation in line with the decision?
E.g., a design/code review or a test with a library such as ArchUnit can help validate this.
Note that although we classify this element as optional, it is included in many ADRs.}
&lt;!-- This is an optional element.
Feel free to remove.
--&gt;
## Pros and Cons of the Options
### {title of option 1}
&lt;!-- This is an optional element.
Feel free to remove.
--&gt;
{example | description | pointer to more information | …}
* Good, because {argument a}
* Good, because {argument b}
&lt;!-- use &quot;neutral&quot; if the given argument weights neither for good nor bad --&gt;
* Neutral, because {argument c}
* Bad, because {argument d}
* … &lt;!-- numbers of pros and cons can vary --&gt;
### {title of other option}
{example | description | pointer to more information | …}
* Good, because {argument a}
* Good, because {argument b}
* Neutral, because {argument c}
* Bad, because {argument d}
* …
&lt;!-- This is an optional element.
Feel free to remove.
--&gt;
## More Information
{You might want to provide additional evidence/confidence for the decision outcome here and/or document the team agreement on the decision and/or define when/how this decision the decision should be realized and if/when it should be re-visited.
Links to other decisions and resources might appear here as well.}
```
> [!cite]- Source> [About MADR](https://adr.github.io/madr/)

### Maintain an architecture decision record (ADR) - Microsoft Learn
### Suggested characteristics of an individual record
- Be consistent with the anatomy of every record.
Design a record template and consistently follow it.
A record should include consistent elements such as:
- Problem statement with context
- Options considered
- Decision outcome
- Include important tradeoffs made with this decision
- Record the confidence level of the decision.
Sometimes an architecturally significant decision is made with relatively low confidence.
Documenting that low confidence status could prove useful for future reconsideration decisions.
> [!cite]- Source · *Oct 9, 2024*> [Maintain an architecture decision record (ADR) - Microsoft Learn](https://learn.microsoft.com/en-us/azure/well-architected/architect-role/architecture-decision-record)

### Simple Decision Log: Decision Timeline &amp; Register for Jira
## Key highlights of the app A lightweight decision log with a visual timeline, impact tracking, and audit trail.
Stop losing decisions in Slack threads
### Never Lose Track of Project Decisions
The visual timeline shows every decision chronologically.
Color-coded status markers (approved/draft/superseded) and impact indicators make it easy to see your project&#39;s decision history at a glance.
### Measure Decision Impact with DACI Framework
Track how decisions affect Schedule, Budget, Scope, Quality, or your custom project areas.
Assign Driver, Approver, Contributors, and Informed roles for clear accountability.
Spot patterns before they become problems.
### Audit Trails and Export into CSV, Markdown and PDF
Link decisions to Jira issues for full traceability.
Export professional PDF reports, CSV data, or Markdown for stakeholder sign-off, audits, and post-mortems.
> [!cite]- Source · *Dec 30, 2025*> [Simple Decision Log: Decision Timeline &amp; Register for Jira](https://marketplace.atlassian.com/apps/1962325789/simple-decision-log-decision-timeline-register-for-jira)

### Engineering Decision Log: The Template That Prevents Repeated ...
Engineering teams make hundreds of decisions every week.
Most of those decisions are never documented.
The result: decisions get reversed, re-made, or contradicted by engineers who did not know the decision had been made — or could not find it when they needed it.
The engineering decision log is one of the highest-leverage practices a distributed team can adopt.
It requires almost no tooling and produces compounding returns as the team&#39;s institutional memory accumulates.
> [!cite]- Source · *Mar 7, 2026*> [Engineering Decision Log: The Template That Prevents Repeated ...](https://www.standin.co/blog/engineering-decision-log-system)

### The Markdown ADR (MADR) Template Explained and Distilled
**Metadata.** The metadata elements are: *status:*
`{proposed | rejected | accepted | deprecated | … | superseded by }`
*date:*
`{YYYY-MM-DD}`when the decision was last updated
*deciders:*lists everyone involved in the decision *consulted:*lists everyone whose opinions are sought and with whom there is a two-way communication (such as subject matter experts) *informed:*lists everyone who is kept up-to-date on progress in one-way communication
…
The template recommends listing the chosen option first (as a project-wide convention).
One needs to make sure to list options that can solve the given problem in the given context (as documented in Section “Context and Problem Statement”).
They should do so on the same level of abstraction; a mistake we have seen in practice is that a technology is compared with a product, or an architectural style with a protocol specification and its implementations.
Pseudo-alternatives sometimes can be found too, but do not help.
> [!cite]- Source · *Nov 21, 2022*> [The Markdown ADR (MADR) Template Explained and Distilled](https://ozimmer.ch/practices/2022/11/22/MADRTemplatePrimer.html)


---

## Conceptual Map

> *How does **Decision records** relate to adjacent concepts?*
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
FROM [[Decision records]]
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

1. [Master architecture decision records (ADRs): Best practices ... - AWS](https://aws.amazon.com/blogs/architecture/master-architecture-decision-records-adrs-best-practices-for-effective-decision-making/) *(updated Apr 1, 2026)*2. [Loqbooq — Free Decision Log for Your Project](https://loqbooq.app) *(updated Apr 4, 2026)*3. [ADR Template | MADR](https://adr.github.io/madr/decisions/adr-template.html) *(updated Jan 27, 2026)*4. [8 best practices for creating architecture decision records | TechTarget](https://www.techtarget.com/searchapparchitecture/tip/4-best-practices-for-creating-architecture-decision-records) *(updated Apr 4, 2026)*5. [About MADR](https://adr.github.io/madr/) *(updated Apr 6, 2026)*6. [Maintain an architecture decision record (ADR) - Microsoft Learn](https://learn.microsoft.com/en-us/azure/well-architected/architect-role/architecture-decision-record) *(updated Mar 31, 2026)*7. [Simple Decision Log: Decision Timeline &amp; Register for Jira](https://marketplace.atlassian.com/apps/1962325789/simple-decision-log-decision-timeline-register-for-jira) *(updated Apr 2, 2026)*8. [Engineering Decision Log: The Template That Prevents Repeated ...](https://www.standin.co/blog/engineering-decision-log-system) *(updated Apr 3, 2026)*9. [The Markdown ADR (MADR) Template Explained and Distilled](https://ozimmer.ch/practices/2022/11/22/MADRTemplatePrimer.html) *(updated Aug 7, 2025)*