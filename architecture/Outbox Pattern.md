Instead of writing to two places, the application writes the business data **and** a "message" into the same database within a single local transaction. A separate process (Relay) then polls this "Outbox" table and sends the message to the external system.

Uses the Atomicity of the local database to ensure the message is only queued if the data is saved.

## Tradeoffs
- **Pros:**
	- Guaranteed eventual consistency
	- no data loss
- **Cons:** 
	- Higher database load (polling)
	- Complexity in managing the Relay service
	- Potential for duplicate messages (requires idempotency)

