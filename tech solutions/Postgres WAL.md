A write-ahead log (WAL) follows a basic principle: **before applying any changes to the main data store, the system writes the changes to an append-only log.** The log serves as a sequential, persistent record of every operation. If the system crashes midway through applying a change, the WAL can be replayed to restore the system to a consistent state.

The idea is straightforward but essential: **you never make a change directly; instead, you first append the change to a durable log.** This guarantees that no matter what happens, the system can always recover or replicate its state.

**Imagine a database table where a row is being updated.** Without a WAL, the database might overwrite the row in the main storage. If the server crashes halfway through writing the new data during this operation, the old and the new data could be corrupted, leaving the system in an inconsistent state. The update is neither “committed” nor safely recoverable.

The WAL solves this by ensuring the following sequence of events:

1. **Log First:** The system writes the change (e.g., “update row X with new value”) to the write-ahead log. This log entry is **sequentially appended** and written for durable storage, such as disks. **That’s why the structure is called Write-Ahead Log, as we’re writing new entries ahead of others.**
2. **Apply Later:** The system applies the change to the actual data structures (e.g., tables or indexes) only after the WAL entry has been safely persisted. This step can be asynchronous and may happen with some delay since the log already guarantees the change is not lost.
3. **Crash Recovery:** If the system crashes after writing the log but before applying the change, the WAL can be replayed on restart. This ensures the operation is eventually applied. The log serves as the source of truth, allowing the system to apply any uncommitted changes and restore a consistent state.

This mechanism guarantees two critical things:
- **Durability:** Changes are not “lost” once they are logged.
- **Consistency:** If a crash occurs, the system can always replay the WAL to apply incomplete operations and recover to a consistent state.