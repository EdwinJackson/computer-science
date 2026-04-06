---
id: iZFn0FaRdrGv_-_8zii_-title: "Process"
tags:
  - concept
  - knowledge-base
created: 2026-04-06source-count: 10---

# Process
> [!abstract] About this note
> Conceptual framework synthesised from **10 sources**.
> Expand each section to deepen the framework.

---

## Definition & Scope

> *What is this concept, and what does it include or exclude?*

## How to Spot a Bottleneck
Before you fix a bottleneck, you have to
*recognize* it.
You can identify bottlenecks in your SDLC by looking for:
### Indicator patterns
**Work queues piling up**before a stage (e.g., code reviews or test environments).
**Cycle times that vary widely or consistently lag targets.** **Frequent rework and sprint interruptions.** **Teams blaming upstream or downstream partners.** **Unplanned work disrupts planned commitments.**
…
### Next steps
**A.
Assess:**
Start with a structured assessment of your SDLC flow.
Where do queues build?
Where does rework repeat?
Which delays undermine predictability?
*Take Iter8’s Assess phase as your next step — it’s designed to diagnose bottlenecks across flow, alignment, and delivery systems.*
**B.
Learn &amp; Measure:**
Track flow metrics regularly.
Use objective data — not opinions — to guide improvement cycles.
**C.
Iterate:**
Fixes should be incremental and measurable.
Small improvements compound into sustained flow gains.
> [!cite]- Primary source
> [The 5 Most Common SDLC Bottlenecks - Iter8 IT Consulting](https://www.iter8itconsulting.com/articles/the-5-most-common-sdlc-bottlenecks) · *Dec 22, 2025*
---

## Key Perspectives

> *How do different sources frame this concept?*

### Working with WIP limits for kanban | Atlassian
Use template
**Key Takeaways**
- WIP (Work-in-Progress) limits the number of tasks in each workflow stage, highlighting bottlenecks and improving workflow efficiency.
- Limiting WIP encourages focus, reduces multitasking, and accelerates delivery by making blockers visible.
- Teams should set, monitor, and adjust WIP limits to optimize throughput and maintain a sustainable pace.
- Implement WIP limits on your kanban board to boost efficiency and foster a culture of completion.
…
## Why are WIP limits important?
...
WIP limits improve throughput and reduce the amount of work &quot;nearly done&quot;, by forcing the team to focus on a smaller set of tasks.
At a fundamental level, WIP limits encourage a culture of &quot;done.&quot;
More important, WIP limits make blockers and bottlenecks visible.
Teams can swarm around blocking issues to get them understood, implemented, and resolved when there is a clear indicator of what existing work is causing a bottleneck.
Once blockages are removed, work across the team begins to flow again.
> [!cite]- Source · *Mar 22, 2026*> [Working with WIP limits for kanban | Atlassian](https://www.atlassian.com/agile/kanban/wip-limits)

### SDLC processes: How to improve the 7 basic methodologies - Waydev
Some key aspects that engineering managers need to pay attention to are the technology and frameworks used and the configuration and implementation principles.
It is equally essential that engineering managers provide their team with the complete requirements and the necessary tools to get the project going.
Every requirement is important at this step, and engineering managers need to look at them separately to ensure no blockages and that the process is running smoothly.
For example, having more observability into your team’s CI/CD processes enables you to eliminate bottlenecks and reduce costs.
> [!cite]- Source · *Sep 7, 2025*> [SDLC processes: How to improve the 7 basic methodologies - Waydev](https://waydev.co/sdlc-processes/)

### Value stream mapping: a complete guide for software engineering ...
## The VSM process
Value stream mapping is a lean management method that visualizes the materials, information, and steps required to deliver software to customers.
It helps teams distinguish between activities that create value and those that introduce waste, providing end-to-end visibility into your software delivery process.
The value stream mapping process relies on four key elements:
**Value stream mapping (VSM)** creates a visual diagram of every step in the software delivery process, surfacing bottlenecks and opportunities for improvement.
A value stream map example might show the flow from feature request through coding, testing, review, and deployment.
…
**Step 3: Designing your future state.** Based on your analysis, create a future state map that envisions a more efficient process.
Focus on reducing waste, removing bottlenecks, and improving flow.
Consider your team structure, technology constraints, and business requirements when designing improvements.
**Step 4: Building an implementation plan.** Translate your future state vision into concrete actions.
Assign ownership for each improvement, establish timelines, and define metrics to measure progress.
Prioritize changes that reduce the most significant sources of friction for developers.
Small improvements in high-frequency activities often deliver more value than large changes to rarely used processes.
> [!cite]- Source> [Value stream mapping: a complete guide for software engineering ...](https://getdx.com/blog/value-stream-analysis/)

### A Tactical Guide to Diagnosing and Resolving Bottlenecks in Kanban
### 3.
Isolate the constraint with smart WIP limiting
When you suspect a bottlenecked process step, impose a stiff WIP limit upstream of that column, then observe what breaks or slows down.
It&#39;s just a diagnostic maneuver, not a fix.
The goal is to trace dependency patterns and uncover hidden constraints, e.g., knowledge silos or resource contention.
***Key move:* **
> [!cite]- Source · *May 25, 2025*> [A Tactical Guide to Diagnosing and Resolving Bottlenecks in Kanban](https://kanbantool.com/blog/resolving-bottlenecks-in-kanban)

### Finding Bottlenecks in your Software Development Lifecycle (SDLC) | Haystack DORA
# Resolving Bottlenecks in your Software Engineering Team
## Step 1: Get a Baseline
First we start by measuring our North Star metrics.
These give us a picture of what the overall performance of the engineering process is.
This should capture sufficient amounts of data to be
*statistically significant*.
Establish a baseline Change Lead Time by looking at the team&#39;s 6 month average.
This tells us how long the average time from first commit to Pull Request merged and will help us diagnose issues that appear between these phases.
## Step 2: Drill Down to Identify Improvement Areas
Next we should seek to understand where the constraints are in the software engineering process.
In the first instance, you can dive into granular metrics to understand what is constraining the North Star metrics.
Is most the Change Lead Time being spent on development time or review time?
How much of the review time is being spent on First Response Time, Rework Time and Idle Completion Time?
> [!cite]- Source · *Oct 17, 2022*> [Finding Bottlenecks in your Software Development Lifecycle (SDLC) | Haystack DORA](https://support.usehaystack.io/en/articles/4523639-finding-bottlenecks-in-your-software-development-lifecycle-sdlc)

### WIP limits explained: boost your workflow efficiency - Miro
### Goal: Expose and eliminate bottlenecks
**Strategy:** Use WIP limits strategically to make constraints visible and force the organization to address them.
- Set WIP limits on downstream stages first (testing, review, deployment) to expose capacity constraints
- When upstream work piles up against a WIP limit, resist the urge to increase the limit — instead, investigate why the bottleneck exists
- Use Miro&#39;s board to visualize where work is accumulating, using the visualization tools to make bottlenecks obvious to stakeholders
- Treat blocked work as an emergency that needs immediate attention
> [!cite]- Source · *Jan 28, 2024*> [WIP limits explained: boost your workflow efficiency - Miro](https://miro.com/kanban/wip-limits-kanban/)

### Development Process And...
- **Manual and repetitive tasks:** If valuable developer time is dedicated to repetitive tasks like testing, deployments, or code reviews, this time is not directly invested in building new functionality.
- **Inefficient workflows and process fragmentation:** Bottlenecks thrive in non-streamlined workflows in the SDLC.
Lengthy code reviews, delayed testing cycles, and fragmented communication channels all complicate the development process.
Studies using DORA and SPACE metrics have emphasized the importance of reducing delays in the inner loop (the core coding and feedback cycle) versus time wasted in the outer loop (integration, deployment, etc.)
- **Outdated or underutilized tooling:** When a team uses outdated tools for source control, CI/CD, monitoring, or collaboration, delays and increased chances for error are expected.
Poorly integrated tools or interleaved manuals can also lead to bottlenecks.
- **Inefficient build and deployment pipelines:** Slow build times or unreliable deployment processes can delay releases and reduce developer morale.
Automation and continuous delivery techniques have often been cited as remedies.
> [!cite]- Source · *Mar 31, 2025*> [Development Process And...](https://mstone.ai/blog/eliminate-engineering-bottlenecks-boost-efficiency/)

### A Guide to Value Stream Mapping in Software Development - Waydev
## Key Takeaways
- Value streams provide a framework for optimizing the process of delivering products, specifically in software development, through Development Value Streams (DVS).
- Value Stream Mapping (VSM) helps organizations visualize the workflow from idea to delivery, improving efficiency and reducing waste.
- Mapping involves identifying steps, using visual representations, and creating current and future state maps to track progress and optimize processes.
…
1. Reducing Cycle Time – you can decrease the time it takes to deliver a working piece of software by using stream mapping.
2. Improving quality – a value stream doesn’t have to stay the same throughout the duration of the deployment process.
Good stream management supported by measuring the most relevant metrics enables you to identify defects and root causes for delays and take action to prevent them from moving forward.
This will ensure a better quality of your deployment processes and of the work needed to bring value to customers.
> [!cite]- Source · *Sep 28, 2025*> [A Guide to Value Stream Mapping in Software Development - Waydev](https://waydev.co/value-stream-mapping/)

### Value stream mapping for software delivery - Dora.dev
Visualizing the flow of work through Value Stream Mapping (VSM) can help improve software delivery performance by enabling shared understanding and empathy regarding the software development process and identifying areas for improvement.
**Flow**, in the context of software development and operations, refers to the smooth and continuous movement of work through the value stream.
When work flows smoothly, it means that there are minimal delays or impediments, leading to faster delivery times and improved efficiency.
Continuous Delivery (CD) is a key enabler of flow, as it focuses on automating the software delivery process and establishing fast feedback loops, allowing teams to release software frequently and reliably.
> [!cite]- Source · *Nov 12, 2024*> [Value stream mapping for software delivery - Dora.dev](https://dora.dev/guides/value-stream-management/)


---

## Conceptual Map

> *How does **Process** relate to adjacent concepts?*
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
FROM [[Process]]
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

1. [The 5 Most Common SDLC Bottlenecks - Iter8 IT Consulting](https://www.iter8itconsulting.com/articles/the-5-most-common-sdlc-bottlenecks) *(updated Jan 19, 2026)*2. [Working with WIP limits for kanban | Atlassian](https://www.atlassian.com/agile/kanban/wip-limits) *(updated Apr 5, 2026)*3. [SDLC processes: How to improve the 7 basic methodologies - Waydev](https://waydev.co/sdlc-processes/) *(updated Apr 5, 2026)*4. [Value stream mapping: a complete guide for software engineering ...](https://getdx.com/blog/value-stream-analysis/) *(updated Apr 5, 2026)*5. [A Tactical Guide to Diagnosing and Resolving Bottlenecks in Kanban](https://kanbantool.com/blog/resolving-bottlenecks-in-kanban) *(updated Mar 21, 2026)*6. [Finding Bottlenecks in your Software Development Lifecycle (SDLC) | Haystack DORA](https://support.usehaystack.io/en/articles/4523639-finding-bottlenecks-in-your-software-development-lifecycle-sdlc) *(updated Oct 30, 2025)*7. [WIP limits explained: boost your workflow efficiency - Miro](https://miro.com/kanban/wip-limits-kanban/) *(updated Apr 2, 2026)*8. [Development Process And...](https://mstone.ai/blog/eliminate-engineering-bottlenecks-boost-efficiency/) *(updated Mar 30, 2026)*9. [A Guide to Value Stream Mapping in Software Development - Waydev](https://waydev.co/value-stream-mapping/) *(updated Mar 27, 2026)*10. [Value stream mapping for software delivery - Dora.dev](https://dora.dev/guides/value-stream-management/) *(updated Apr 5, 2026)*