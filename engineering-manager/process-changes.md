---
id: ev9ZKygqETctLMSt1GAFUtitle: "Process changes"
tags:
  - concept
  - knowledge-base
created: 2026-04-06source-count: 8---

# Process changes
> [!abstract] About this note
> Conceptual framework synthesised from **8 sources**.
> Expand each section to deepen the framework.

---

## Definition & Scope

> *What is this concept, and what does it include or exclude?*

## Identifying Improvement Opportunities
Start by observing where your team loses time.
Common sources of waste include: waiting for code reviews, context switching between too many concurrent projects, meetings that lack clear agendas or outcomes, manual processes that could be automated, and unclear ownership that leads to duplicated effort or dropped responsibilities.
Use both quantitative and qualitative signals.
Cycle time metrics, deployment frequency, and code review turnaround times provide objective data.
Retrospective feedback, one-on-one conversations, and your own observations provide context that numbers alone cannot capture.
The best process improvements address issues that show up in both the data and the lived experience of your team.
Prioritise improvements that reduce recurring friction.
A process improvement that saves each engineer thirty minutes per week is more valuable than one that saves five hours on a one-time event.
Focus on the processes your team uses daily or weekly, not the ones that only matter quarterly.
- Track cycle time, deployment frequency, and code review turnaround as baseline metrics
- Listen to retrospective themes for qualitative signals of process friction
- Prioritise improvements that address daily or weekly recurring pain points
- Look for manual processes that can be automated with minimal investment
## Implementing Process Changes
The most important principle of process improvement is to change one thing at a time.
Implementing multiple process changes simultaneously makes it impossible to determine which change had what effect.
It also overwhelms your team with adaptation overhead.
Choose the highest-impact improvement, implement it, measure the result, and then move on to the next one.
Involve your team in the design of process changes.
Changes imposed from above generate resistance; changes co-created with the team generate ownership.
Present the problem you have identified, share the data that supports it, and ask the team to help design the solution.
You may be surprised by how often the team produces a better solution than the one you had in mind.
Run process changes as experiments with defined success criteria.
Instead of permanently changing how the team works, frame the change as a two-week experiment.
At the end of the experiment, evaluate whether the change achieved its goals and decide together whether to keep it, modify it, or revert it.
This reduces the psychological cost of trying new things because the team knows the change is reversible.
…
## Key Takeaways
- Focus on improvements that reduce recurring daily or weekly friction
- Change one process at a time and measure the impact before moving on
- Involve your team in designing process changes to build ownership
- Frame changes as reversible experiments to reduce resistance
- Remove existing overhead before adding new processes
…
- **Should engineering managers drive process improvement or delegate it to the team?**
Both.
The engineering manager is responsible for identifying systemic process issues and ensuring the team has the time and support to address them.
But the team should own the design and implementation of specific improvements.
Your role is to create the conditions for continuous improvement - dedicated time, psychological safety to experiment, and follow-through on commitments - not to dictate every process detail.
> [!cite]- Primary source
> [Process Improvement for Engineering Managers: A Complete Guide](https://www.em-tools.io/engineering-manager-responsibilities/process-improvement) · *Mar 5, 2026*
---

## Key Perspectives

> *How do different sources frame this concept?*

### 7 process improvement methodologies to improve efficiency
|**Methodology**|**Best for**|**Key focus**|
|--|--|--|
|Six Sigma|Reducing defects|Data-driven quality control|
|TQM|Customer satisfaction|Organization-wide quality|
|Lean manufacturing|Eliminating waste|Value stream optimization|
|Kaizen|Incremental change|Continuous small improvements|
|PDCA|Testing solutions|Iterative problem-solving|
|5 Whys|Root cause analysis|Identifying process errors|
|BPM|Scaling operations|End-to-end process management|
Create a process map template
> [!cite]- Source · *Jan 12, 2026*> [7 process improvement methodologies to improve efficiency](https://asana.com/resources/process-improvement-methodologies)

### Engineering Change Management Process Overview | PTC
- Easily configured change processes that scale to meet business needs
- Flexible workflows that get the right tasks to the right users
- Streamlined interactions with changes
- Easy-to-understand reviews that meet the particular needs of different roles
- Improved change validation to ensure that business rules are met
- Mass updates, setting effectivity and planning supersedes
> [!cite]- Source> [Engineering Change Management Process Overview | PTC](https://www.ptc.com/en/blogs/plm/engineering-change-management-process-overview)

### How to Improve the Productivity of Your Engineering Team
- Share knowledge across teams and locations
- Assign experienced mentors to new team members
- Give teams access to software that will help them do their jobs accurately
- Get feedback from engineers on where training efforts would be placed best
**Pro tip**: By implementing effective training processes tailored to the specific needs of your engineers, you can ensure that your team is developing the skills, knowledge and experience it needs to be successful long-term.
> [!cite]- Source · *Sep 30, 2022*> [How to Improve the Productivity of Your Engineering Team](https://www.h2xengineering.com/blogs/how-to-improve-the-productivity-of-your-engineering-team/)

### Software Change Management: Best Practices &amp; Tools for 2026
### Agile methodologies
Agile change management is designed to accommodate frequent and incremental software updates.
It’s best suited for product-focused teams and iterative development.
#### How agile change management works
Instead of a centralized approval board (as seen in ITIL), Agile change management is handled within cross-functional development teams.
**Changes are managed through:**
- **Scrum-based sprint cycles: ** Changes are broken down into smaller, manageable work units and implemented in short development cycles (sprints).
- **Kanban workflows:** Continuous, visual task management where changes flow from development to testing and deployment as soon as they’re ready.
- **Backlog grooming &amp; prioritization: ** Changes are reviewed, prioritized, and added to the backlog based on business and customer needs.
**Since agile teams deploy changes frequently, they rely heavily on:**
- **Automated testing** to catch issues early.
- **Version control (e.g., Git)** to track changes and allow easy rollbacks.
- **Incremental deployments** rather than large, disruptive releases.
DevOps builds on this by fully automating change management through CI/CD pipelines, automated testing in staging environments, and incremental rollout strategies like canary and blue-green deployments.
### Waterfall model
The Waterfall model follows a linear, sequential approach to software development and change management.
Changes progress through strict, predefined phases.
Each phase must be completed before the next begins.
**The typical phases include:**
1. **Requirement gathering &amp; analysis: ** Defining software specifications and identifying potential future changes.
2. **Design: ** Creating a detailed architecture to accommodate possible changes.
3. **Implementation: ** Writing code according to the specifications.
4. **Testing: ** Verifying that all components work correctly.
5. **Deployment: ** Releasing the software after all changes are finalized.
…
#### How change management works in Waterfall models
Unlike Agile and DevOps, which embrace frequent, iterative changes, Waterfall front-loads all change management activities into the planning phase.
‍
Modifications in later stages (especially after deployment) require a full review, approval, and sometimes a complete restart of development phases.
And without continuous integration, even minor updates must follow a structured approval and testing process to avoid breaking dependencies.
> [!cite]- Source · *Jan 28, 2026*> [Software Change Management: Best Practices &amp; Tools for 2026](https://www.superblocks.com/blog/software-change-management)

### Sustaining Change Over The...
New CI/CD pipeline.
New team structure.
New process for handling on-call.
Engineering managers drive change constantly - and most of it fails because the change was imposed rather than introduced.
Your team does not resist improvement; they resist being told to change their habits without understanding why.
This guide gives you a practical framework for leading transitions that stick: building genuine buy-in, managing the resistance that always appears, and sustaining the change past the initial enthusiasm.
…
For engineering managers, the Lewin model is often the most practical: Unfreeze (create readiness for change by helping people understand why the current state is unsustainable), Change (implement the new approach with support and resources), and Refreeze (stabilise the new approach through reinforcement and habit formation).
This simple three-stage model provides enough structure without the complexity of larger frameworks.
…
- Kotter&#39;s eight-step model provides a comprehensive roadmap for large-scale change
- ADKAR focuses on individual change through Awareness, Desire, Knowledge, Ability, and Reinforcement
- Lewin&#39;s Unfreeze-Change-Refreeze model is practical for team-level engineering changes
- People resist being changed, not change itself - involvement and communication are key
> [!cite]- Source · *Mar 5, 2026*> [Sustaining Change Over The...](https://www.em-tools.io/frameworks/change-management)

### 10 Change Management Models: Options, Tips, And Diagrams
At the core of the model is a structured workflow: logging the change, assessing its risk and potential impact, getting it reviewed (often by a Change Advisory Board or CAB), implementing it in a controlled way, and then closing it with a review.
Roles like the Change Manager support the process, which is often integrated with ITSM tools to maintain audit trails and ensure coordination across departments.
…
## 8.
Agile Change Management model
This model applies Agile principles to Change Management efforts.
Rather than treating change as a one-time rollout, it supports incremental adjustments, quick feedback loops, and flexibility.
It typically includes:
- Rolling out change in small, testable increments
- Using feedback from teams and users to adjust continuously
- Encouraging self-managed teams to take ownership
- Prioritizing working solutions over long plans
> [!cite]- Source · *May 6, 2025*> [10 Change Management Models: Options, Tips, And Diagrams](https://invgate.com/itsm/change-management/change-management-models)

### Making process changes as an engineering manager
An engineering team’s formal processes — how you track sprints, run meetings, handle release cadence, and manage code reviews — helps set team velocity and impacts the happiness of individual team members.
As the engineering manager, you’re in an impactful role to shape and improve these processes over time.
**Remember when making any change in process, be patient yet firm.**
> [!cite]- Source · *Mar 3, 2019*> [Making process changes as an engineering manager](https://www.nickschaden.com/2019/03/04/making-process-changes-as-an-engineering-manager/)


---

## Conceptual Map

> *How does **Process changes** relate to adjacent concepts?*
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
FROM [[Process changes]]
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

1. [Process Improvement for Engineering Managers: A Complete Guide](https://www.em-tools.io/engineering-manager-responsibilities/process-improvement) *(updated Apr 1, 2026)*2. [7 process improvement methodologies to improve efficiency](https://asana.com/resources/process-improvement-methodologies) *(updated Apr 6, 2026)*3. [Engineering Change Management Process Overview | PTC](https://www.ptc.com/en/blogs/plm/engineering-change-management-process-overview) *(updated Mar 30, 2026)*4. [How to Improve the Productivity of Your Engineering Team](https://www.h2xengineering.com/blogs/how-to-improve-the-productivity-of-your-engineering-team/) *(updated Mar 10, 2026)*5. [Software Change Management: Best Practices &amp; Tools for 2026](https://www.superblocks.com/blog/software-change-management) *(updated Mar 18, 2026)*6. [Sustaining Change Over The...](https://www.em-tools.io/frameworks/change-management) *(updated Apr 4, 2026)*7. [10 Change Management Models: Options, Tips, And Diagrams](https://invgate.com/itsm/change-management/change-management-models) *(updated Apr 1, 2026)*8. [Making process changes as an engineering manager](https://www.nickschaden.com/2019/03/04/making-process-changes-as-an-engineering-manager/) *(updated Jul 21, 2025)*