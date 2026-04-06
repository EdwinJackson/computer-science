---
id: pduPcv2QPpVmVvDdK4CPititle: "System Monitoring &amp; Performance"
tags:
  - concept
  - knowledge-base
created: 2026-04-06source-count: 9---

# System Monitoring &amp; Performance
> [!abstract] About this note
> Conceptual framework synthesised from **9 sources**.
> Expand each section to deepen the framework.

---

## Definition & Scope

> *What is this concept, and what does it include or exclude?*

#### Key Takeaways
1. **The Four Golden Signals** — latency, traffic, errors, and saturation — are core metrics for monitoring and maintaining system health in SRE practices.
2. **Tracking these signals** alongside SLIs, SLOs, and SLAs within a unified framework enables teams to set clear targets for performance and availability.
> [!cite]- Primary source
> [SRE Metrics: Core SRE Components, the Four Golden Signals ...](https://www.splunk.com/en_us/blog/learn/sre-metrics-four-golden-signals-of-monitoring.html) · *Feb 24, 2025*
---

## Key Perspectives

> *How do different sources frame this concept?*

### 10 Best Infrastructure Monitoring Tools in 2025 - Kloudfuse
# List of The Best Infrastructure Monitoring Tools
1. ​​Kloudfuse
2. Datadog Infrastructure Monitoring
3. New Relic
4. Dynatrace
5. Grafana Cloud
6. LogicMonitor
7. Splunk Observability Cloud
8. Zabbix
9. Prometheus
10. Nagios XI
> [!cite]- Source · *Apr 1, 2026*> [10 Best Infrastructure Monitoring Tools in 2025 - Kloudfuse](https://www.kloudfuse.com/blog/infrastructure-monitoring-tools)

### What are SLOs, SLAs, and SLIs? A complete guide to service reliability ...
|Availability Target|Monthly Downtime|Annual Downtime|Use Case|
|--|--|--|--|
|99%|7.2 hours|3.65 days|Development environments|
|99.9%|43.8 minutes|8.76 hours|Standard web applications|
|99.95%|21.9 minutes|4.38 hours|Business-critical SaaS|
|99.99%|4.38 minutes|52.56 minutes|High-availability services|
|99.999%|26.3 seconds|5.26 minutes|Mission-critical systems|
…
## Quick reference: SLI vs SLO vs SLA comparison table
...
|Aspect|**SLI (Service Level Indicator)**|
|--|--|
|**Definition**|The actual, real-time measurement of your service performance.
It&#39;s the raw data that tells you exactly how your system is performing right now.|
|**Metrics examples**|- **Availability**: 99.97% uptime measured over last 30 days - **Latency**: P95 response time = 187ms - **Error rate**: 0.03% failed requests - **Throughput**: 52,341 requests/second - **Durability**: 99.999999999% data integrity|
> [!cite]- Source · *Aug 24, 2025*> [What are SLOs, SLAs, and SLIs? A complete guide to service reliability ...](https://incident.io/blog/slo-sla-sli)

### SRE best practices 2026: tips, tools and KPIs - Just After Midnight
- **Cost of downtime:** The calculated revenue lost per unit of time during a service outage based on historical transaction averages.
- **Customer impact score:** A weighted measurement of the total number of users affected by an incident multiplied by the business criticality of the failed function.
- **SLA compliance rate:** The percentage of time the service met its contractual uptime obligations to avoid financial penalties or service credits.
…
- **SLO attainment:** Success rate over a rolling window (e.g., 28 days).
- **User error rate:** % of requests that fail for users (per critical journey).
- **Tail latency (*p95/p99)*:** The experience of your most frustrated users.
At scale, the average latency is a lie; the *p99* is the truth.
…
- ***p95 * Time to mitigate (TTM):** How long it takes to restore service for the vast majority of incidents.
(Avoid mean times, as outliers skew the data).
- **Time to detect (TTD):** The gap between user impact and system awareness.
- **Toil rate:** The amount of interrupt-driven manual work.
If SREs spend *&gt;50\% * of their time on tickets vs. engineering, the system is unsustainable.
> [!cite]- Source · *Feb 5, 2026*> [SRE best practices 2026: tips, tools and KPIs - Just After Midnight](https://www.justaftermidnight247.com/insights/site-reliability-engineering-sre-best-practices-2026-tips-tools-and-kpis/)

### What is a service-level objective (SLO)? SLO vs. SLA vs. SLI
If your SLA includes a 99.9% uptime guarantee, your SLO should reflect that.
Aiming for 99.9% uptime over 30 days means you’re limited to 43.2 minutes of downtime over a month.
You can use uptime monitoring services to track your uptime and downtime throughout the month.
> [!cite]- Source · *Dec 9, 2025*> [What is a service-level objective (SLO)? SLO vs. SLA vs. SLI](https://www.atlassian.com/incident-management/kpis/sla-vs-slo-vs-sli)

### Top SRE KPI Metrics to Improve Availability &amp; Reliability
**Mean Time to Acknowledge (MTTA)**
This metric reflects your on-call efficiency.
It measures how quickly engineers acknowledge alerts.
Slow responses usually hint at alert fatigue or overloaded teams.
**Mean Time to Resolve (MTTR)**
MTTR determines how long it takes to fully resolve an incident and restore normal service.
It’s one of the strongest indicators of operational maturity.
…
...
##
The most important SRE KPI metrics include availability, MTTR, error rate, latency, and change failure rate because they directly impact system reliability and user satisfaction.
> [!cite]- Source · *Nov 19, 2025*> [Top SRE KPI Metrics to Improve Availability &amp; Reliability](https://www.novelvista.com/blogs/devops/sre-kpi-metrics)

### 15 Best Infrastructure Monitoring Tools in 2026 - Dash0
Grafana is the ideal choice for teams that have embraced a **Prometheus monitoring** philosophy and prioritize a world-class visualization experience.
If you have the engineering muscle to manage the self-hosted stack, it offers ultimate control.
If you opt for Grafana Cloud, be prepared to wrestle with the alerting system and keep a very close eye on your usage to avoid surprise costs.
> [!cite]- Source · *Jun 29, 2025*> [15 Best Infrastructure Monitoring Tools in 2026 - Dash0](https://www.dash0.com/comparisons/infrastructure-monitoring-tools)

### 18 SRE Metrics Worth Tracking (And Why) - OneUptime
## A.
User Experience &amp; SLO Health
|Metric|Why|Trigger|
|--|--|--|
|**Availability SLI (per journey)**|Captures user-visible uptime|Burn rate &gt; 2× for 1h → investigate|
|**Latency P95/P99 (per journey)**|Exposes tail pain that averages hide|P99 &gt; target for 3 intervals → rollback or add capacity|
|**Error Budget Remaining**|Balances speed vs safety|&lt;50% mid-period → slow risky deploys|
|**Synthetic Success Rate**|Validates critical flows proactively|Drop &gt;2% → check recent changes|
> [!cite]- Source · *Nov 27, 2025*> [18 SRE Metrics Worth Tracking (And Why) - OneUptime](https://oneuptime.com/blog/post/2025-11-28-sre-metrics-to-track/view)

### SLOs, SLIs, and SLAs: Meanings &amp; Differences | New Relic
| |SLA|SLO|SLI|
|--|--|--|--|
|**Examples**|**Will deliver**: 99.99% uptime; two hour resolution time.
Minimum 12-hour recovery from data loss.
**Failure to perform**: Payment credits per unit of time.|Response time less than or equal to 300ms; error rate less than 2%; 3 copies of data.|Average response time = 250.1ms.
Uptime percentage = 98.9%|
|**Typical influencers**|Customer, business group, legal department|System architect, system integrator, reliability engineering team|Reliability engineering team|
...
### Examples of SLIs
SLIs serve as the foundation upon which SLOs and SLAs are based.
Let’s look at some examples.
**Availability/Uptime**
- Percentage of successful requests vs. total requests.
- Ratio of system uptime to the total time period.
**Latency**
- Time taken for an API request to return a response.
- Time taken for a web page to load for the end user.
> [!cite]- Source · *Dec 17, 2024*> [SLOs, SLIs, and SLAs: Meanings &amp; Differences | New Relic](https://newrelic.com/blog/observability/what-are-slos-slis-slas)


---

## Conceptual Map

> *How does **System Monitoring &amp; Performance** relate to adjacent concepts?*
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
FROM [[System Monitoring &amp; Performance]]
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

1. [SRE Metrics: Core SRE Components, the Four Golden Signals ...](https://www.splunk.com/en_us/blog/learn/sre-metrics-four-golden-signals-of-monitoring.html) *(updated Apr 5, 2026)*2. [10 Best Infrastructure Monitoring Tools in 2025 - Kloudfuse](https://www.kloudfuse.com/blog/infrastructure-monitoring-tools) *(updated Apr 4, 2026)*3. [What are SLOs, SLAs, and SLIs? A complete guide to service reliability ...](https://incident.io/blog/slo-sla-sli) *(updated Apr 5, 2026)*4. [SRE best practices 2026: tips, tools and KPIs - Just After Midnight](https://www.justaftermidnight247.com/insights/site-reliability-engineering-sre-best-practices-2026-tips-tools-and-kpis/) *(updated Apr 6, 2026)*5. [What is a service-level objective (SLO)? SLO vs. SLA vs. SLI](https://www.atlassian.com/incident-management/kpis/sla-vs-slo-vs-sli) *(updated Apr 4, 2026)*6. [Top SRE KPI Metrics to Improve Availability &amp; Reliability](https://www.novelvista.com/blogs/devops/sre-kpi-metrics) *(updated Apr 6, 2026)*7. [15 Best Infrastructure Monitoring Tools in 2026 - Dash0](https://www.dash0.com/comparisons/infrastructure-monitoring-tools) *(updated Apr 3, 2026)*8. [18 SRE Metrics Worth Tracking (And Why) - OneUptime](https://oneuptime.com/blog/post/2025-11-28-sre-metrics-to-track/view) *(updated Mar 26, 2026)*9. [SLOs, SLIs, and SLAs: Meanings &amp; Differences | New Relic](https://newrelic.com/blog/observability/what-are-slos-slis-slas) *(updated Apr 4, 2026)*