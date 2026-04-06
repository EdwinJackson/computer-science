---
id: fYkKo8D35AHd8agr3YrIPtitle: "Blameless Post-mortems"
tags:
  - concept
  - knowledge-base
created: 2026-04-06source-count: 10---

# Blameless Post-mortems
> [!abstract] About this note
> Conceptual framework synthesised from **10 sources**.
> Expand each section to deepen the framework.

---

## Definition & Scope

> *What is this concept, and what does it include or exclude?*

Blameless postmortems are a tenet of SRE culture.
For a postmortem to be truly blameless, it must focus on identifying the contributing causes of the incident without indicting any individual or team for bad or inappropriate behavior.
A blamelessly written postmortem assumes that everyone involved in an incident had good intentions and did the right thing with the information they had.
If a culture of finger pointing and shaming individuals or teams for doing the &quot;wrong&quot; thing prevails, people will not bring issues to light for fear of punishment.
Blameless culture originated in the healthcare and avionics industries where mistakes can be fatal.
These industries nurture an environment where every &quot;mistake&quot; is seen as an opportunity to strengthen the system.
When postmortems shift from allocating blame to investigating the systematic reasons why an individual or team had incomplete or incorrect information, effective prevention plans can be put in place.
You can’t &quot;fix&quot; people, but you can fix systems and processes to better support people making the right choices when designing and maintaining complex systems.
> [!cite]- Primary source
> [Blameless Postmortem for System Resilience - Google SRE](https://sre.google/sre-book/postmortem-culture/)
---

## Key Perspectives

> *How do different sources frame this concept?*

### Postmortem Practices for Incident Management - Google SRE
###### Blamelessness
The authors focused on the gaps in system design that permitted undesirable failure modes.
For example:
Things that went poorly
- No individual or team is blamed for the incident.
Root cause and trigger
- Focuses on “what” went wrong, not “who” caused the incident.
Action items
- Are aimed at improving the system instead of improving people.
…
###### Use blameless language
Blameful language stifles collaboration between teams.
Consider the following scenario:
- Sandy missed a service Foo training and wasn’t sure how to run a particular update command.
The delay ultimately prolonged an outage.
- SRE Jesse [to Sandy’s manager]: “You’re the manager; why aren’t you making sure that everyone finishes the training?”
> [!cite]- Source> [Postmortem Practices for Incident Management - Google SRE](https://sre.google/workbook/postmortem-culture/)

### Etsy Engineering | Blameless PostMortems and a Just Culture
So what do we do to enable a &quot;Just Culture&quot; at Etsy?
- We encourage learning by having these blameless Post-Mortems on outages and accidents.
- The goal is to understand **how **an accident could have happened, in order to better equip ourselves from it happening in the future
- We seek out Second Stories, gather details from multiple perspectives on failures, and we don&#39;t punish people for making mistakes.
- Instead of punishing engineers, we instead give them the requisite authority to improve safety by allowing them to give detailed accounts of their contributions to failures.
- We enable and encourage people who *do* make mistakes to be the experts on educating the rest of the organization how not to make them in the future.
- We accept that there is always a discretionary space where humans can decide to make actions or not, and that the judgement of those decisions lie in hindsight.
> [!cite]- Source · *May 21, 2012*> [Etsy Engineering | Blameless PostMortems and a Just Culture](https://www.etsy.com/codeascraft/blameless-postmortems)

### How to run a blameless postmortem | Atlassian
### Encourage honesty and acceptance of failure
The detractors who say blameless postmortems don’t have enough accountability?
Here’s where they’re wrong.
Your postmortems should encourage honesty and accountability.
Removing the fear of consequences frees people up to be honest about their missteps and misunderstandings.
And that’s the only way to fix them.
> [!cite]- Source · *Dec 9, 2025*> [How to run a blameless postmortem | Atlassian](https://www.atlassian.com/incident-management/postmortem/blameless)

### How to implement a Blameless Postmortem (part two) · Raygun Blog
- A facilitator enforces rules of behavior.
In particular, counterfactual language like “could have”, “should have”, etc that promotes the illusion of one single (human) point of failure.
- Every postmortem should have at least one short- and one long-term action or remediation work item (i.e. not all incidents are repeatable or deserve a full postmortem).
…
Some rules of thumb from the excellent SRE workbook by Google:
- Are the action items realistic and vetted with product owners?
- Have you considered ways to improve both prevention and resolution time?
- Have you considered similar or “rhyming” incidents and their corresponding action plans?
- Have you considered how to automate ways to prevent humans from making mistakes?
- Does your postmortem have at least one Critical Priority or High Priority action item?
If not, is the risk of recurrence accepted by stakeholders?
- Have you negotiated the execution of action items with the responsible group(s)?
> [!cite]- Source · *Apr 5, 2022*> [How to implement a Blameless Postmortem (part two) · Raygun Blog](https://raygun.com/blog/blameless-postmortems-part-two/)

### The Blameless Postmortem
An organization that follows this old view of human error may respond to an incident by finding the careless individual who caused the incident so they can be reprimanded.
**This impulse to blame and punish has the unintended effect of disincentivizing the knowledge sharing required to prevent future failure.** Engineers will hesitate to speak up when incidents occur for fear of being blamed.
This silence increases overall mean time to acknowledge, mean time to resolve, and exacerbates the impact of incidents.
…
** A blameless postmortem stays focused on *how* a mistake was made instead of *who* made it.
This is a crucial mindset leveraged by many leading organizations (such as Etsy, a pioneer for blameless postmortems) for ensuring postmortems have the right tone, empowering engineers to give truly objective accounts of what happened by eliminating the fear of punishment.
…
## How to Cultivate a Blameless (or Blame-Aware) Culture #
Acknowledging blame and working past it is easier said than done.
What behaviors can we adopt to move towards a blameless culture?
Holmwood eloquently writes about the importance of the words we use to minimize blame and maximize learning.
He urges us to ask “what” questions (e.g., “What did you think was happening?” and “What did you do next?”
Asking “what” questions grounds the analysis in the big-picture contributing factors to the incident.
…
Key Takeaways
- Ask “what” and “how” questions rather than “who” or “why.”
- Consider multiple and diverse perspectives.
- Ask yourself why a reasonable, rational, and decent person may have taken a particular action.
- When inquiring about a human action, abstract to an inspecific responder.
Anyone could have made the same mistake.
- Restore mutual purpose and mutual respect by contrasting what you did not intend with what you do intend.
> [!cite]- Source> [The Blameless Postmortem](https://postmortems.pagerduty.com/culture/blameless/)

### Blameless Postmorterm Guideline
## Postmortem Templates and Samples
## Do’s
- Focus on identifying the contributing causes of the incident without indicting any individual or team for bad or inappropriate behavior
- Assume everyone involved in an incident had good intentions and did the right thing with the information they had at the time
- See every “mistake” as an opportunity to strengthen the system
- Create a culture of continuous improvement
- Have it asap so that timelines and activities are fresh in peoples memory
- Involve everyone that participated in the troubleshooting and resolution and also everyone with an interest
- Be open, listen to input
- Share your post-mortem with others
> [!cite]- Source · *Dec 31, 2018*> [Blameless Postmorterm Guideline](https://esdc-devcop.github.io/guides/postmortem.html)

### Etsy&#39;s Winning Secret: Don&#39;t Play the Blame Game! - Business Insider
In another example, a developer broke the system which let users favorite, or bookmark, items they were thinking about buying.
&quot;Less-skilled companies name, blame, and shame,&quot; said Allspaw.
It&#39;s not about avoiding accountability.
In a blameless culture, it&#39;s easier for people to take responsibility for their mistakes and learn from them.
…
**3 TIPS FROM ETSY ON ADOPTING A BLAMELESS CULTURE:**
- **Assume good will.
** &quot;Employees are making decisions based on what they think is right for the company,&quot; said Allspaw.
- **Identify causes, not culprits.** Accountability happens naturally as people learn the facts.
Focus on exploring what happened—and recognize that in complex systems, there&#39;s rarely one root cause.
- **Take your time.
** People used to blaming cultures may take time to come out of their shell and share mistakes and learnings freely.
> [!cite]- Source · *May 14, 2012*> [Etsy&#39;s Winning Secret: Don&#39;t Play the Blame Game! - Business Insider](https://www.businessinsider.com/etsy-chad-dickerson-blameless-post-mortem-2012-5)

### Blameless Post-mortem Culture: How To Improve Learning and ...
At its core, a blameless postmortem culture is a practice where, when incidents occur, teams focus on what happened within
the system, rather than assigning fault to specific individuals.
Instead of asking “who did this,” teams ask:
1. What signals did we see (or miss)?
2. What assumptions did we make at the time?
3. What constraints were people operating under?
4. How did tooling, processes, or communication contribute?
> [!cite]- Source> [Blameless Post-mortem Culture: How To Improve Learning and ...](https://phoenixincidents.com/blog/blameless-post-mortem-culture-how-to-improve-learning)

### Kitchen Soap – Learning from Failure at Etsy
So what do we do to enable a “Just Culture” at Etsy?
- We encourage learning by having these blameless Post-Mortems on outages and accidents.
- The goal is to understand
**how**an accident could have happened, in order to better equip ourselves from it happening in the future
- We seek out Second Stories, gather details from multiple perspectives on failures, and we don’t punish people for making mistakes.
- Instead of punishing engineers, we instead give them the
> [!cite]- Source> [Kitchen Soap – Learning from Failure at Etsy](https://www.kitchensoap.com/2013/09/30/learning-from-failure-at-etsy/)


---

## Conceptual Map

> *How does **Blameless Post-mortems** relate to adjacent concepts?*
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
FROM [[Blameless Post-mortems]]
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

1. [Blameless Postmortem for System Resilience - Google SRE](https://sre.google/sre-book/postmortem-culture/) *(updated Apr 6, 2026)*2. [Postmortem Practices for Incident Management - Google SRE](https://sre.google/workbook/postmortem-culture/) *(updated Mar 26, 2026)*3. [Etsy Engineering | Blameless PostMortems and a Just Culture](https://www.etsy.com/codeascraft/blameless-postmortems) *(updated Jan 16, 2026)*4. [How to run a blameless postmortem | Atlassian](https://www.atlassian.com/incident-management/postmortem/blameless) *(updated Apr 5, 2026)*5. [How to implement a Blameless Postmortem (part two) · Raygun Blog](https://raygun.com/blog/blameless-postmortems-part-two/) *(updated Mar 7, 2026)*6. [The Blameless Postmortem](https://postmortems.pagerduty.com/culture/blameless/) *(updated Mar 12, 2026)*7. [Blameless Postmorterm Guideline](https://esdc-devcop.github.io/guides/postmortem.html) *(updated Jan 13, 2026)*8. [Etsy&#39;s Winning Secret: Don&#39;t Play the Blame Game! - Business Insider](https://www.businessinsider.com/etsy-chad-dickerson-blameless-post-mortem-2012-5) *(updated Mar 4, 2026)*9. [Blameless Post-mortem Culture: How To Improve Learning and ...](https://phoenixincidents.com/blog/blameless-post-mortem-culture-how-to-improve-learning) *(updated Apr 1, 2026)*10. [Kitchen Soap – Learning from Failure at Etsy](https://www.kitchensoap.com/2013/09/30/learning-from-failure-at-etsy/) *(updated Aug 28, 2025)*