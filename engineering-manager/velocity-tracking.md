---
id: idd92ZTBVUzptBl5jRdc3title: "Velocity Tracking"
tags:
  - concept
  - knowledge-base
created: 2026-04-06source-count: 9---

# Velocity Tracking
> [!abstract] About this note
> Conceptual framework synthesised from **9 sources**.
> Expand each section to deepen the framework.

---

## Definition & Scope

> *What is this concept, and what does it include or exclude?*

### Focusing on team predictability
I believe **seeking and achieving team predictability – understanding the capacity of work for the team over a period of time – is the most important thing we can focus on outside of core needs to increase team resiliency**.
Once we have data around the team’s capacity, it becomes a finite data point.
Our prioritization conversations then shift to how we can maximize impact given that capacity.
This can lead us to further simplify MVPs, reprioritize less-impactful work to make space, and it prevents excess pressure on the team to hit an unrealistic deadline, because we set those deadlines with data.
…
We also need to **address disruptions or escalations that may get in the way**.
In software engineering, work can be nearly impossible to reliably predict, and so we always need to leave space to handle the unexpected.
If your team works in sprints, planning to 80% of the team’s capacity can be a good baseline, adjusting as needed based on how much uncertainty there is in the team’s work.
This leaves space for escalations, unexpected absences, and mispointed work.
…
**When setting timelines for project completion, we can use our predicted capacity as a guideline**, determining the number of sprints it will take when planning to 80% (or your percentage of choice), but I find it helpful to provide an additional buffer for the unexpected, where that buffer length is set based on the overall risk and complexity of the project.
> [!cite]- Primary source
> [Focusing On Team...](https://www.shelly-stuart.com/blog/breaking-the-burnout-cycle-in-efficient-engineering-teams) · *Oct 15, 2023*
---

## Key Perspectives

> *How do different sources frame this concept?*

### Does high velocity lead to burnout? That may be the wrong question ...
For better or worse, different teams come up with different ways to define these points and measure them.
However, the most popular way tends to be folks on the product side come up with work that is framed out with clear criteria, and then devs as a group “size” this work with how much effort they think it will take with a number we call story points.
So the work is planned, developers measure how much work they *think * it will be with a number (story points), and the sum of the number of points in the work they complete in an interval is their velocity.
…
Then the hedging and compromising start.
Folks will begin to rationalize the long tiresome hours to justify the numbers getting bigger on a spreadsheet.
Then, as we alluded to in the beginning, the inevitable burnout starts.
All team members, not just developers, begin to realize they aren’t making good decisions; they are going down the wrong path but this arbitrary velocity number is the one defining what is right or wrong.
> [!cite]- Source · *Aug 21, 2022*> [Does high velocity lead to burnout? That may be the wrong question ...](https://stackoverflow.blog/2022/08/22/does-high-velocity-lead-to-burnout-that-may-be-the-wrong-question-to-ask/)

### Engineering Resource Planning: Best Practices for ... - Jellyfish
### Step 4: Implement the Right Resource Optimization Techniques and Pivot When Needed
Engineering projects are often dynamic, with unexpected challenges and changing priorities.
As a result, you should track resource utilization and task progress throughout your project to proactively identify issues, such as bottlenecks and burnout, and adjust plans.
If your project hits a speed bump, consider deploying these two resource optimization techniques:
- **Resource smoothing:** Re-adjust task assignments to distribute workload evenly and prevent overloading critical engineers.
- **Resource leveling** **:** Extend deadlines or re-allocate tasks to balance workload when projects are not time-sensitive.
…
- **Monitor workload carefully:** Use resource management tools, developer experience tools, dashboards, and regular check-ins to track individual workloads and identify potential overallocation.
- **Utilize resource leveling and smoothing techniques:** Distribute workload evenly across the team and avoid overloading critical engineers.
- **Promote work-life balance:** Encourage healthy work habits, provide adequate time off, and foster a supportive work environment.
> [!cite]- Source · *Feb 3, 2025*> [Engineering Resource Planning: Best Practices for ... - Jellyfish](https://jellyfish.co/blog/engineering-resource-planning/)

### Why Preventing Burnout Is Essential for Growth Engineering Teams
### 1.
Prioritize Workload with Realistic Sprint Goals
Leverage data-driven prioritization frameworks such as RICE (Reach, Impact, Confidence, Effort) or ICE (Impact, Confidence, Ease) to balance urgency and impact.
Involve engineers actively in sprint planning and regularly review sprint velocity to adjust goals and prevent overcommitment.
…
## Implementing Burnout Prevention Strategies: Step-by-Step Guidance
### 1.
Prioritize Workload with Realistic Sprint Goals
- Apply RICE or ICE scoring during backlog grooming to rank tasks objectively.
- Engage engineers in sprint planning to set achievable commitments.
- Track sprint velocity trends and adjust scope to avoid consistent spillovers.
> [!cite]- Source> [Why Preventing Burnout Is Essential for Growth Engineering Teams](https://www.zigpoll.com/content/how-can-i-effectively-implement-burnout-prevention-strategies-within-a-highpressure-growth-engineering-team-to-maintain-productivity-and-morale-in-a-competitive-environment)

### Beyond story points: how to measure developer velocity the right way
When developers are measured in terms of units of output, they tend to disengage.
Frustration grows as metrics are manipulated, fueling the retention crisis in engineering.
The human cost is just as real.
Developers choose this profession to solve complex problems and build products that matter.
Reducing their work to points or lines of code undermines the motivation that drives their best contributions.
…
This framework prevents single-metric optimization, which can destroy traditional velocity measurement.
Teams can’t game speed at the expense of quality or boost activity metrics while ignoring the business impact.
This comprehensive approach is why organizations implementing the DX Core 4 see a 3%-12% overall increase in engineering efficiency, 14% increase in R&amp;D time spent on feature development, and 15% improvement in employee engagement scores.
### Outcome-based measurement
Modern agile software development velocity requires moving beyond story point tracking toward outcome-based measurement.
The Core 4 framework enables agile teams to:
- Track actual delivery speed (speed dimension) rather than estimated story points
- Measure developer satisfaction and workflow efficiency (effectiveness dimension)
- Ensure sustainable pace through quality metrics (quality dimension)
- Connect sprint work to business value (business impact dimension)
…
### John Lewis: 40% more coding time through experience optimization
John Lewis moved beyond story point velocity to measure actual developer effectiveness.
Their comprehensive approach focused on reducing friction through workflow automation, process standardization, tool optimization, and quality integration.
Business impact: 40% increase in time spent coding and 10x+ ROI on developer experience investments.
> [!cite]- Source> [Beyond story points: how to measure developer velocity the right way](https://getdx.com/blog/developer-velocity/)

### Beyond speed: Measuring engineering success by impact, not velocity
And on teams that emphasize velocity over all other considerations, burnout is an inevitability.
Engineers are asked to do more and more without truly understanding where their work is making a difference.
...
It’s clear to many leaders that when engineering teams begin to feel burnout, the ripples of that are felt throughout the organization.
> [!cite]- Source · *May 11, 2025*> [Beyond speed: Measuring engineering success by impact, not velocity](https://stackoverflow.blog/2025/05/12/beyond-speed-measuring-engineering-success-by-impact-not-velocity/)

### Engineering Resource Planning: Steps &amp; Best Practices for A&amp;E Firms
Watch for the common pitfall of leaning on your top performers until they crack.
A bi-weekly rebalancing meeting solves it: drag-and-drop assignments in Monograph&#39;s resource planner, preview utilization charts, and redistribute.
The result feels less like crisis triage and more like tuning a well-engineered structure.
Firms tracking resource allocation in real-time achieve 4x faster billing cycles.
> [!cite]- Source · *Aug 24, 2025*> [Engineering Resource Planning: Steps &amp; Best Practices for A&amp;E Firms](https://monograph.com/blog/engineering-resource-planning)

### Boost Team Morale With Velocity Tracking
Furthermore, without understanding the team&#39;s capacity and previous performance, planning future sprints becomes a guessing game.
This can lead to either underestimating the team&#39;s capabilities, resulting in missed opportunities, or overestimating, leading to burnout and increased stress.
The ability to accurately predict future performance based on historical data is crucial for effective resource allocation and project planning.
This is where the power of velocity tracking truly shines, providing valuable insights that empower teams to make informed decisions and optimize their workflow.
…
Furthermore, velocity tracking allows for early detection of potential problems.
By monitoring the team&#39;s velocity over time, it&#39;s possible to identify trends that may indicate underlying issues.
For example, a gradual decline in velocity could be a sign of burnout, technical debt, or process inefficiencies.
By identifying these issues early on, it&#39;s possible to take corrective action before they escalate into major problems.
This proactive approach not only protects the team&#39;s productivity but also demonstrates a commitment to their well-being, which further strengthens team morale.
> [!cite]- Source · *Apr 24, 2025*> [Boost Team Morale With Velocity Tracking](https://tribes.gitscrum.com/unleash-team-synergy-velocity-tracking-drives-engineering-morale-skyward/)

### Ship Fast, Stay Human: Developer Velocity Without Burnout - Code ...
### The velocity–burnout paradox
Pushing hours and counting commits does not create velocity.
It creates frustration.
Developers can burn out even at
**20 to 30** hours per week if those hours are spent firefighting, context switching, and doing repetitive work.
Real velocity is measured in outcomes.
If a team ships **20** low-impact features and misses one high-value release, it did not move fast.
It moved sideways.
> [!cite]- Source · *Nov 17, 2025*> [Ship Fast, Stay Human: Developer Velocity Without Burnout - Code ...](https://codeandconscience.com/blog/shipping-fast-staying-human-velocity-without-burnout)


---

## Conceptual Map

> *How does **Velocity Tracking** relate to adjacent concepts?*
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
FROM [[Velocity Tracking]]
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

1. [Focusing On Team...](https://www.shelly-stuart.com/blog/breaking-the-burnout-cycle-in-efficient-engineering-teams) *(updated Mar 14, 2026)*2. [Does high velocity lead to burnout? That may be the wrong question ...](https://stackoverflow.blog/2022/08/22/does-high-velocity-lead-to-burnout-that-may-be-the-wrong-question-to-ask/) *(updated Mar 18, 2026)*3. [Engineering Resource Planning: Best Practices for ... - Jellyfish](https://jellyfish.co/blog/engineering-resource-planning/) *(updated Mar 27, 2026)*4. [Why Preventing Burnout Is Essential for Growth Engineering Teams](https://www.zigpoll.com/content/how-can-i-effectively-implement-burnout-prevention-strategies-within-a-highpressure-growth-engineering-team-to-maintain-productivity-and-morale-in-a-competitive-environment) *(updated Mar 7, 2026)*5. [Beyond story points: how to measure developer velocity the right way](https://getdx.com/blog/developer-velocity/) *(updated Mar 30, 2026)*6. [Beyond speed: Measuring engineering success by impact, not velocity](https://stackoverflow.blog/2025/05/12/beyond-speed-measuring-engineering-success-by-impact-not-velocity/) *(updated Mar 29, 2026)*7. [Engineering Resource Planning: Steps &amp; Best Practices for A&amp;E Firms](https://monograph.com/blog/engineering-resource-planning) *(updated Apr 3, 2026)*8. [Boost Team Morale With Velocity Tracking](https://tribes.gitscrum.com/unleash-team-synergy-velocity-tracking-drives-engineering-morale-skyward/) *(updated Jun 27, 2025)*9. [Ship Fast, Stay Human: Developer Velocity Without Burnout - Code ...](https://codeandconscience.com/blog/shipping-fast-staying-human-velocity-without-burnout) *(updated Nov 22, 2025)*