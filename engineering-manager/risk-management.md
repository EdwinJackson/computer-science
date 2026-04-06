---
id: mgw6M8I9qy1EoJpJV-gy1title: "Risk Management"
tags:
  - concept
  - knowledge-base
created: 2026-04-06source-count: 9---

# Risk Management
> [!abstract] About this note
> Conceptual framework synthesised from **9 sources**.
> Expand each section to deepen the framework.

---

## Definition & Scope

> *What is this concept, and what does it include or exclude?*

## Risk Mitigation Strategies
Common mitigation strategies include avoidance (changing plans to eliminate the risk), reduction (taking steps to lower the likelihood or impact), transfer (shifting the risk to another party, such as through insurance or vendor agreements), and acceptance (acknowledging the risk and preparing to manage it if it occurs).
For technical risks, common mitigations include prototyping to validate uncertain technology choices, building abstraction layers to reduce dependency on specific technologies, implementing feature flags for safe rollouts, and maintaining rollback capabilities.
For people risks, cross-training, documentation, and succession planning are the primary mitigations.
…
## Key Takeaways
- Identify risks proactively through pre-mortems and regular risk reviews
- Assess risks on likelihood and impact to prioritise mitigation efforts
- Choose proportionate mitigation strategies - not every risk needs elimination
- Build a culture where raising risks early is valued and encouraged
- Keep risk management lightweight and practical, not bureaucratic
> [!cite]- Primary source
> [Risk Management: An Engineering Manager&#39;s Guide - EM Tools](https://www.em-tools.io/engineering-manager-responsibilities/risk-management) · *Mar 5, 2026*
---

## Key Perspectives

> *How do different sources frame this concept?*

### [PDF] Contingency planning guide
progressive steps are designed to consider risk management principles and the integration 
of security into each stage of the system development life cycle.
•  Develop the contingency planning policy statement.
A formal policy provides the 
authority and guidance necessary to develop an effective contingency plan.
The 
contingency planning policy statement should define the organization’s overall
> [!cite]- Source> [[PDF] Contingency planning guide](https://tsapps.nist.gov/publication/get_pdf.cfm?pub_id=906210)

### Risk Management Strategies in Engineering Projects
**Contingency Planning:** One of the most critical aspects of risk mitigation is preparing for unforeseen events.
Developing contingency plans for key risks ensures that the team is ready to respond quickly and effectively when challenges arise.
These plans should include predefined actions, additional resources, and time buffers.
> [!cite]- Source · *Feb 10, 2025*> [Risk Management Strategies in Engineering Projects](https://www.kiernanengineering.com/risk-management-strategies-in-engineering-projects/)

### Risk Management Framework: A Guide for Engineering Managers
## Risk Mitigation Strategies for Engineering Teams
The four standard mitigation strategies are: avoid (change plans to eliminate the risk), reduce (take action to lower the likelihood or impact), transfer (shift the risk to a third party through insurance, contracts, or managed services), and accept (acknowledge the risk and prepare to respond if it materialises).
Most engineering risks are addressed through reduction or acceptance.
…
Use risks to inform estimation.
If a project has significant technical uncertainty, add a contingency buffer to the timeline.
The size of the buffer should be proportional to the risk level - a well-understood project might need ten percent contingency, while a project with novel technology might need thirty to fifty percent.
Communicate this uncertainty to stakeholders using ranges rather than point estimates.
> [!cite]- Source · *Mar 5, 2026*> [Risk Management Framework: A Guide for Engineering Managers](https://www.em-tools.io/frameworks/risk-management)

### How to Create a Contingency Plan for Project Success - TrueProject
### Practical Steps for Building a Proactive Contingency Plan Framework
Proactive contingency planning requires a deliberate, structured framework integrating predictive capabilities into everyday project activities.
Here’s a step-by-step guide to help organizations build a system that doesn’t just react to risks but anticipates and neutralizes them before they escalate:
**Step 1: Identify and Prioritize Key Risks**
Start by conducting a comprehensive risk assessment to identify potential threats across critical dimensions—budget, schedule, resources, and quality.
Assign risk scores based on potential impact and likelihood to ensure teams stay focused on the most important risks.
**Step 2: Establish Real-Time Monitoring Systems**
Set up systems that continuously monitor live project performance metrics.
These systems should automatically flag deviations from expected performance, such as cost overruns or task delays, triggering immediate review and action.
**Step 3: Develop Scenario-Based Action Plans**
Develop scenario-based action plans by modelling different risk events—such as supply chain disruptions or workforce shortages—and outlining the exact steps teams should take in response.
…
**Step 6: Conduct Regular Contingency Plan Reviews**
Schedule periodic reviews to update risk assumptions, recalibrate predictive models, and adjust action plans based on lessons learned from past projects.
By following these steps, organizations can build a contingency planning framework that is agile, predictive, and highly responsive to project dynamics.
> [!cite]- Source · *Feb 19, 2025*> [How to Create a Contingency Plan for Project Success - TrueProject](https://www.trueprojectinsight.com/blog/project-office/contingency-plan)

### How to Make a Risk Management Plan (Template Included)
- **Risk mitigation strategies:** Proactive actions designed to reduce the likelihood or impact of identified risks.
In a risk management plan, these strategies help minimize disruptions, protect project objectives, guide resource allocation, support contingency planning and provide structured responses to uncertainty before risks escalate.
- **Risk management roles and responsibilities:** Define who identifies, owns, monitors and responds to risks throughout the project.
Clearly assigned responsibilities—from the project manager and risk owners to stakeholders and support teams—ensure accountability, consistent risk oversight and effective execution of risk response actions.
…
|**Risk ID**|**Risk Description**|**Risk Mitigation Strategy**|**Response Type**|**Roles and Responsibilities**|
|--|--|--|--|--|
|R-01|Unexpected subsurface conditions|Conduct early geotechnical surveys and include contingency plans|Mitigate|Project manager coordinates studies and approvals|
|R-02|Concrete supply delays|Prequalify alternate suppliers and place early orders|Mitigate|Procurement lead manages supplier agreements|
|R-03|Severe weather impacts|Build schedule buffers and resequence non-critical work|Accept|Site supervisor adjusts daily work plans|
|R-04|Safety incidents during elevated work|Implement enhanced safety training and inspections|Avoid|Safety officer enforces compliance and reporting|
> [!cite]- Source · *Dec 14, 2025*> [How to Make a Risk Management Plan (Template Included)](https://www.projectmanager.com/blog/risk-management-plan)

### Risk Register Template
• Risk Statement or Description – The description should contain detail sufficient to assess risk impact and provide project Stakeholders with an understanding of risk to the project.
Risk Statement = Concern + Likelihood + Consequence.,,,,,,,,,
• Date Risk Identified – Enter the date the risk was added to the Risk Register.,,,,,,,,,
> [!cite]- Source> [Risk Register Template](https://www.ucop.edu/information-technology-services/_files/itlc/3.4-supporting-doc-risk-register-template-with-instructions.xlsx)

### What Is Contingency Planning? Creating a Contingency Plan
### 1.
Identify Key Business Processes and Resources
To create an effective contingency plan you should first identify what are the key processes and resources that allow your organization to reach its business goals.
This will help you understand what risks could be the most impactful to your organization.
Research your company and list its crucial processes such as supply chain management or production planning as well as key resources, such as teams, tools, facilities, etc., then prioritize that list from most important to least important.
> [!cite]- Source · *Jul 18, 2023*> [What Is Contingency Planning? Creating a Contingency Plan](https://www.projectmanager.com/blog/contingency-plan)

### Risk register template: Free guide &amp; download for 2025
1. **Risk category:** The type of risk
2. **Risk name:** A brief description of the risk so that people can easily understand what risk you are assessing.
3. **Impact: ** Description of the potential impacts should the risk occur, ideally in business terms.
Decide whether to use “worst case” or “anticipated” impacts and be consistent.
Consistency is especially important as the risk register gets larger and more people get involved in the assessments.
4. **Impact rating or score:** The product of the probability and impact values, or in other words, the untreated/inherent level of risk.
5. **Treatment: ** Description of how the risk is to be treated.
This is often a written statement detailing the plan of action
6. **Treatment status:** To what extent is the planned treatment in place?
0% means the treatment is only a plan at present; nothing has been done about it yet.
100% means that the treatment is fully operational.
…
### Identify risks
Identifying risks is the foundation of your entire risk register.
This step involves gathering key team members, those directly involved in the project and stakeholders who will feel the impact and conducting a collaborative brainstorming session.
During this session, consider internal and external factors that could derail the project’s timeline, budget, scope, or quality.
Think broadly: risks can be technical (e.g., system failures), organizational (e.g., staffing changes), regulatory (e.g., compliance requirements), or even reputational (e.g., public backlash).
…
When the supplier notifies the team of a delay in router shipment, the risk owner refers to the register and implements the backup plan: switching to an alternate vendor pre-vetted in the mitigation notes.
The project continues with only minimal disruption.
Weekly review meetings include updates to the risk register, which now acts as both a tracking tool and communication hub.
With the structured template, the IT team maintains full visibility into risks and responses, ultimately completing the upgrade on time and under budget.
The risk register template proves to be an essential, living document throughout the project lifecycle.
> [!cite]- Source · *Jul 1, 2025*> [Risk register template: Free guide &amp; download for 2025](https://www.trustcloud.ai/risk-management/guide-on-creating-a-risk-register-template/)


---

## Conceptual Map

> *How does **Risk Management** relate to adjacent concepts?*
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
FROM [[Risk Management]]
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

1. [Risk Management: An Engineering Manager&#39;s Guide - EM Tools](https://www.em-tools.io/engineering-manager-responsibilities/risk-management) *(updated Mar 20, 2026)*2. [[PDF] Contingency planning guide](https://tsapps.nist.gov/publication/get_pdf.cfm?pub_id=906210) *(updated Feb 18, 2026)*3. [Risk Management Strategies in Engineering Projects](https://www.kiernanengineering.com/risk-management-strategies-in-engineering-projects/) *(updated Apr 4, 2026)*4. [Risk Management Framework: A Guide for Engineering Managers](https://www.em-tools.io/frameworks/risk-management) *(updated Apr 1, 2026)*5. [How to Create a Contingency Plan for Project Success - TrueProject](https://www.trueprojectinsight.com/blog/project-office/contingency-plan) *(updated Apr 2, 2026)*6. [How to Make a Risk Management Plan (Template Included)](https://www.projectmanager.com/blog/risk-management-plan) *(updated Mar 31, 2026)*7. [Risk Register Template](https://www.ucop.edu/information-technology-services/_files/itlc/3.4-supporting-doc-risk-register-template-with-instructions.xlsx) *(updated Mar 31, 2026)*8. [What Is Contingency Planning? Creating a Contingency Plan](https://www.projectmanager.com/blog/contingency-plan) *(updated Apr 4, 2026)*9. [Risk register template: Free guide &amp; download for 2025](https://www.trustcloud.ai/risk-management/guide-on-creating-a-risk-register-template/) *(updated Mar 25, 2026)*