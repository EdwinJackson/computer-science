The **Dual-Write Problem** is a classic challenge in distributed systems that occurs when an application needs to update two different systems—typically a database and a search index (like Elasticsearch) or a message broker (like Kafka)—as part of a single logical operation.

Since most databases and external systems don't share a unified transaction manager, you cannot guarantee that both writes will succeed or fail together.

## The Core Issue

If your code looks like this:
1. **Update Database** (Succeeds)
2. **Update Search Index** (Fails)

Your systems are now out of sync. If you reverse the order, the same risk applies. This leads to **data inconsistency**, which is often difficult and expensive to repair manually.

| **Pattern**                 | **Consistency** | **Complexity** | **Performance Impact** |
| --------------------------- | --------------- | -------------- | ---------------------- |
| **Dual-Write (Naive)**      | None            | Low            | High Risk              |
| **[[Outbox Pattern]]**      | Eventual        | Medium         | Minimal (DB overhead)  |
| **[[Change Data Capture]]** | Eventual        | High           | Lowest (non-invasive)  |
| **[[Listen to Yourself]]**  | Eventual        | High           | Higher Latency         |
