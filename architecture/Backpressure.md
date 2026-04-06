A control-flow mechanism where a producer is creating events faster than a consumer can process them. 

Instead of letting the data overflow and crash the system (like a flood), backpressure pushes back against the source, forcing it to slow down or buffering the work until the consumer catches up.

**Analogy:** Imagine a sink.
- **The Faucet (Producer):** Pours water (data/events) into the sink.
- **The Drain (Consumer):** Processes the water.
- **No Backpressure:** If the faucet is fully open and the drain is narrow, the sink overflows (System Crash/Out of Memory).
- **With Backpressure**: you partially close the faucet or use a larger basin to temporarily hold the water, ensuring the water level never spills over.

