---
id: q5SJyM1d8cQzzAcR-kotBtitle: "Testing Strategies"
tags:
  - concept
  - knowledge-base
created: 2026-04-06source-count: 14---

# Testing Strategies
> [!abstract] About this note
> Conceptual framework synthesised from **14 sources**.
> Expand each section to deepen the framework.

---

## Definition & Scope

> *What is this concept, and what does it include or exclude?*

identified, the team can allocate more testing resources 
and time to that area.
Another important application is in 
continuous integration and continuous delivery (CI/CD) 
pipelines.
By integrating RBT into CI/CD, teams can 
ensure that high-risk code changes are tested 
thoroughly before being deployed to production (Smith,
…
leading to improved product quality and accelerated 
release cycles.
The integration of RBT into the agile 
workflow, including sprint planning (Smith, 2023) and 
CI/CD pipelines (Taylor, 2022), facilitates continuous risk 
assessment and adaptation, ensuring that testing 
priorities remain aligned with evolving requirements and
> [!cite]- Primary source
> [[PDF] Fail Fast, Fix Faster: Risk-Based Testing for Agile Product Teams](https://engineeringresearch.org/index.php/GJRE/article/download/101743/17039/34694)
---

## Key Perspectives

> *How do different sources frame this concept?*

### Levels of Automation in Software Testing - QATestLab Blog
## Three-level model of Test Automation strategy
Test automation engineers divide automated testing into three levels:
1. Unit Tests / Component Tests
At this level, automated tests are the component of unit tests designed by developers.
Testers can also write such tests if they have the necessary skills.
Tests in the early stages of the project, as well as their constant actualization and the addition of new tests, checking the “bug fixes”, can help to protect the project from the many serious problems.
…
## Possible models for test automation according to its degree
To have a complete picture of the organization of the automation process on a project, let’s look at its model capabilities in terms of the degree of automation.
Possible levels of test automation can be divided and described as follows:
**Level 1** Assistance.
The expert writes a test that should be supported.
It’s useful to make all changes visible.
So, we are doing here simple checking phases and a visual check of the front-end.
**Level 2** Partial Automation.
It’s a phase of still test writing.
Yes, we still check and analyze everything, but AI is helping us here.
**Level 3** Conditional Automation.
Here AI checks every change in tests and deploys the necessary upgrades.
**Level 4** High Automation.
It’s time for AI to write tests under QA engineer’s control and decide what functionality autotests must cover and where they should be applied.
**Level 5** Full Automation.
Complete AI responsibility for writing and supporting tests without human interaction at all.
> [!cite]- Source · *Aug 18, 2015*> [Levels of Automation in Software Testing - QATestLab Blog](https://blog.qatestlab.com/2015/08/19/test-automation-levels/)

### Risk-Based Testing Guide: Strategy, Matrix &amp; Real Examples
Many modern applications are highly complex and require a lot of testing.
However, QA and development teams often lack the time and resources to test every program component.
Thanks to risk-based testing, they can solve this potential problem and focus on the software’s most critical areas that require attention.
By prioritizing tests based on risk, organizations can optimize their testing processes, reduce the likelihood of critical failures, and deliver software that meets both technical and business requirements.
Furthermore, **they achieved 35% higher ROI** on their test investments **according to a 2023 study.**
> [!cite]- Source · *Jun 5, 2025*> [Risk-Based Testing Guide: Strategy, Matrix &amp; Real Examples](https://testomat.io/blog/risk-based-testing/)

### A Practical Approach to Risk-Based Testing
### Risk-Based Testing in Agile
Risk-based testing aligns seamlessly with agile methodologies, enhancing the effectiveness of testing in iterative and fast-paced development environments.
In Agile, where rapid iterations and frequent changes are the norm, risk-based testing helps prioritize testing efforts based on changing requirements and evolving risks.
It allows teams to adapt testing strategies quickly and efficiently, ensuring that critical functionalities are thoroughly tested within each iteration.
…
- **Identify and Assess Risks**: Begin by identifying potential risks associated with the software, considering factors such as impact, likelihood, and criticality.
Assess each risk based on its severity and relevance to the project.
- **Prioritize Testing Efforts**: Once risks are identified and assessed, prioritize testing efforts based on the level of risk.
Focus on areas with higher risks, ensuring that critical functionalities and potential failure points are thoroughly tested.
> [!cite]- Source · *Jul 2, 2023*> [A Practical Approach to Risk-Based Testing](https://www.ranorex.com/blog/risk-based-testing-approach/)

### Test Strategy: How To Create One [Template + Examples]
## What To Include in a Test Strategy Document
### 1.
Test level
Start your test strategy with the concept of a test pyramid, which consists of 3 levels:
- **Unit tests (Base)** – Test individual components in isolation.
Fast, automated, and high in coverage (70-80%).
- **Integration tests (Middle)** – Verify data flow between components.
Moderate speed and coverage (15-20%).
- **E2E tests (Top)** – Validate the full system.
Slow, complex, but crucial for key workflows (5-10%).
> [!cite]- Source · *Jun 20, 2023*> [Test Strategy: How To Create One [Template + Examples]](https://katalon.com/resources-center/blog/test-strategy)

### Continuous Testing Strategies for CI/CD - Library
A comprehensive guide to continuous testing strategies in CI/CD pipelines, covering the testing pyramid, shift-left testing, test selection by pipeline stage, quality gates, test impact analysis, progressive validation, risk-based testing, and building a testing culture that scales with delivery speed.
ci-cdazure-devopstest-planscontinuous-testingtesting-strategyquality-gates
…
- **Match test investment to risk.** Payment processing, authentication, and data integrity deserve more testing investment than cosmetic features.
Use risk-based test selection to run more tests for high-risk changes and fewer for low-risk ones.
- **Measure and reduce feedback cycle time.** Track the time from commit to first test result (commit stage duration) and from commit to production deployment (total pipeline duration).
Set targets and optimize.
Every minute saved from the feedback loop pays dividends across every developer on every commit.
> [!cite]- Source · *Feb 12, 2026*> [Continuous Testing Strategies for CI/CD - Library](https://www.grizzlypeaksoftware.com/library/continuous-testing-strategies-for-cicd-myfnmv7g)

### Optimize CI Pipelines with AI Risk-Based Testing | DEVOPSdigest
Example for CI Optimization
An E2E testsuite with 1,000 tests running through a CI pipeline in 10 parallel threads takes 60 minutes to complete.
60 minutes is a long time.
...
Inserting an AI risk-based testing tool into the pipeline would allow it to auto-select and execute only the tests relevant to developer changes, and thereby reduce the number of tests needing to be executed.
In this example, if Smart Test Selection is set at 10%, it would prioritize the top 100 E2E tests for execution based on the recent developer commits.
The execution time would drop from 60 minutes down to approximately 6 minutes to complete.
By adding an AI risk-based testing tool into the CI pipeline, the team can now run against the full 1,000 tests while AI picks the top 100 tests given a recent change on a per PR basis to save time and resources.
A worthy option to consider over just throwing more hardware at the issue.
> [!cite]- Source · *Jun 5, 2023*> [Optimize CI Pipelines with AI Risk-Based Testing | DEVOPSdigest](https://www.devopsdigest.com/optimize-ci-pipelines-with-ai-risk-based-testing)

### Types of Automated Testing Explained Within Test Strategy
## Levels of automated testing
Testing is divided into four levels, depending on how comprehensive software testing is:
…
- **Integration testing.** Various software components are combined and tested during this type of testing.
This provides an opportunity to see if the new module integrates correctly with the common code base and interacts with other components.
- **System Testing.** This is a comprehensive test of the software product functioning as a single system.
By running different types of testing for different program modules, QA engineers find out how the finished application meets the stated requirements.
> [!cite]- Source · *Jun 22, 2023*> [Types of Automated Testing Explained Within Test Strategy](https://testomat.io/blog/types-of-automated-testing-explained-within-test-strategy/)

### Software Testing Strategies: A Practical Guide for QA Teams in 2026
### The hybrid approach
Most mature teams use a hybrid strategy.
They automate stable, repetitive checks that run in CI/CD pipelines, freeing up human testers to focus on exploratory testing, usability evaluation, and complex scenarios that are expensive to automate and prone to change.
The key metric is not &quot;percentage of tests automated.&quot;
It is whether your testing strategy efficiently catches the bugs that matter before users find them.
> [!cite]- Source · *Feb 19, 2026*> [Software Testing Strategies: A Practical Guide for QA Teams in 2026](https://testcollab.com/blog/software-testing-strategies)

### Understanding the Pros and Cons of Risk-Based Testing
#### Prioritize testing based on risks
When planning sprints, focus on high-risk features first.
Critical issues are addressed early to keep the software delivery-ready after each sprint.
**Image: ** TestRail enables teams to assign priorities and categorize tests based on risk levels.
This allows for better planning and allocation of resources to critical areas, aligning with RBT principles.
…
#### Use risks as a guiding light for your CI/CD
Continuously test an application’s high-risk areas using risks as the roadmap for your CI/CD pipeline.
This helps maintain software quality and high-priority risk coverage in every sprint.
> [!cite]- Source · *Feb 15, 2026*> [Understanding the Pros and Cons of Risk-Based Testing](https://www.testrail.com/blog/risk-based-testing/)

### The Complete Guide to Software Testing Types, Levels, Strategies ...
## Test Levels: Where Testing Happens in the Lifecycle
Test levels define where testing is performed in the hierarchy—from code to customer acceptance.
Common levels include:
- Unit testing (logic and functions)
- Component or contract testing (modules or APIs)
- Integration testing (interfaces and workflows)
- System testing (overall application behavior)
- Acceptance testing (user, operational, and regulatory validation)
- Alpha and beta testing (real-world or field environments)
…
## Risk-Based Testing Strategy: How Decisions Are Made
A risk-based strategy begins with identifying threats and mapping them to quality attributes.
It specifies where those risks can be best mitigated and how testing should be prioritized.
The process follows a consistent flow:
- Define risks and quality characteristics
- Choose the lowest effective test levels
- Select appropriate design techniques and coverage metrics
- Establish static and dynamic testing balance
- Automate where possible
- Define measurable acceptance criteria such as SLOs or CVSS thresholds
> [!cite]- Source · *Nov 3, 2025*> [The Complete Guide to Software Testing Types, Levels, Strategies ...](https://talent500.com/blog/complete-guide-software-testing-types-levels-strategies/)

### Developing a Powerful Test Automation Strategy
### Integrating Automation into the CI/CD Pipeline
- **WHAT it is:** A tiered strategy for running the right tests at the right time to get fast, relevant feedback without slowing down development.
- **WHY it matters:** Running a 45-minute E2E test suite on every commit would bring development to a halt.
A tiered approach intelligently balances the need for speed with the need for confidence.
> [!cite]- Source · *Oct 14, 2025*> [Developing a Powerful Test Automation Strategy](https://dev.to/idavidov13/developing-a-powerful-test-automation-strategy-frameworks-cicd-e2e-tests-1916)

### Agile Testing Methodology - Life Cycle &amp; Best Practices
## Strategies for Effective Agile Testing
### Risk-Based Testing
Risk-based testing in agile focuses effort where failures would have greatest impact.
Critical features receive comprehensive testing.
Stable features receive lighter validation.
New integrations receive extra attention.
Complex changes receive thorough examination.
This prioritisation ensures testing resources deliver maximum value rather than spreading evenly across all features.
The assessment of risk in agile happens continuously rather than upfront.
Each sprint evaluates risk based on changes, dependencies, and business impact.
Testing strategies adjust based on emerging information.
Resource allocation follows risk priorities.
This continuous assessment ensures testing focus remains aligned with actual rather than perceived risks.
> [!cite]- Source · *Jan 5, 2022*> [Agile Testing Methodology - Life Cycle &amp; Best Practices](https://www.virtuosoqa.com/post/what-is-agile-testing)

### Software Testing Types, Approaches, Levels, and ...
### 2.
Test levels (where in the lifecycle?)￼
Test level categorises where tests are written in the system hierarchy/lifecycle (unit -&gt; integration -&gt; system -&gt; acceptance).
Different levels expose different fault classes: unit/component work is best at catching local logic errors and boundary conditions; integration/contract work reveals interface and protocol mismatches; system testing exposes end-to-end behavior, configuration, and cross-cutting concerns; acceptance/field testing validates suitability for users, operations, and regulations.
Keeping these levels distinct speeds feedback where it’s cheapest (lower levels) and reserves slower, costlier runs for risks that only appear at higher scopes.
…
It also enables parallelization and CI gates (explicit entry/exit criteria per level), makes coverage and traceability interpretable (map each requirement/risk to the lowest effective level and choose techniques accordingly), satisfies compliance obligations that demand evidence at specific levels (e.g., FAT/SAT/OAT, UAT sign-off), and reinforces risk-based selection so teams don’t try to catch everything with slow, brittle end-to-end tests.
> [!cite]- Source · *Oct 28, 2025*> [Software Testing Types, Approaches, Levels, and ...](https://qase.io/blog/software-testing-types-approaches-levels-execution-strategies-and-techniques-the-complete-guide/)


---

## Conceptual Map

> *How does **Testing Strategies** relate to adjacent concepts?*
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
FROM [[Testing Strategies]]
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

1. [[PDF] Fail Fast, Fix Faster: Risk-Based Testing for Agile Product Teams](https://engineeringresearch.org/index.php/GJRE/article/download/101743/17039/34694) *(updated Mar 3, 2026)*2. [Levels of Automation in Software Testing - QATestLab Blog](https://blog.qatestlab.com/2015/08/19/test-automation-levels/) *(updated Oct 29, 2025)*3. [Risk-Based Testing Guide: Strategy, Matrix &amp; Real Examples](https://testomat.io/blog/risk-based-testing/) *(updated Apr 6, 2026)*4. [A Practical Approach to Risk-Based Testing](https://www.ranorex.com/blog/risk-based-testing-approach/) *(updated Mar 12, 2026)*5. [Test Strategy: How To Create One [Template + Examples]](https://katalon.com/resources-center/blog/test-strategy) *(updated Apr 6, 2026)*6. [Continuous Testing Strategies for CI/CD - Library](https://www.grizzlypeaksoftware.com/library/continuous-testing-strategies-for-cicd-myfnmv7g) *(updated Mar 14, 2026)*7. [Optimize CI Pipelines with AI Risk-Based Testing | DEVOPSdigest](https://www.devopsdigest.com/optimize-ci-pipelines-with-ai-risk-based-testing) *(updated Nov 19, 2025)*8. [Types of Automated Testing Explained Within Test Strategy](https://testomat.io/blog/types-of-automated-testing-explained-within-test-strategy/) *(updated Apr 4, 2026)*9. [Software Testing Strategies: A Practical Guide for QA Teams in 2026](https://testcollab.com/blog/software-testing-strategies) *(updated Apr 6, 2026)*10. [Understanding the Pros and Cons of Risk-Based Testing](https://www.testrail.com/blog/risk-based-testing/) *(updated Mar 12, 2026)*11. [The Complete Guide to Software Testing Types, Levels, Strategies ...](https://talent500.com/blog/complete-guide-software-testing-types-levels-strategies/) *(updated Mar 27, 2026)*12. [Developing a Powerful Test Automation Strategy](https://dev.to/idavidov13/developing-a-powerful-test-automation-strategy-frameworks-cicd-e2e-tests-1916) *(updated Nov 13, 2025)*13. [Agile Testing Methodology - Life Cycle &amp; Best Practices](https://www.virtuosoqa.com/post/what-is-agile-testing) *(updated Mar 24, 2026)*14. [Software Testing Types, Approaches, Levels, and ...](https://qase.io/blog/software-testing-types-approaches-levels-execution-strategies-and-techniques-the-complete-guide/) *(updated Apr 5, 2026)*