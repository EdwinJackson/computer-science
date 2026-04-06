> AkA State Machine Replication

The message broker becomes the "source of truth."

The application sends a message to a broker (like Kafka) _first_. The application then consumes its own message to update its local database, while the search index also consumes that same message.

## Tradeoffs
- **Pros:** 
	- Both systems receive the same sequence of events.     
- **Cons:** 
	- Increased latency for the user (read-after-write consistency becomes harder)
	- When the message broker is down, the app cannot update its own database