**Context:** Ingestion creates many small files (the "small files problem"), causing massive metadata overhead and slow read performance for downstream consumers.

**Solution:** Run a job that coalesces small files into larger, optimal ones. Modern table formats (Delta, Iceberg) have native commands (`OPTIMIZE`).

**Challenges:**

- **Cost vs. Latency:** Running compaction too often wastes compute; too rarely hurts read performance.
- **Cleaning:** Compaction creates new files; old files must be removed (e.g., `VACUUM`) to reclaim storage.

**Python/Delta Lake**

```python
from delta.tables import *

# Compact small files
devices_table = DeltaTable.forPath(spark_session, table_dir)
devices_table.optimize().executeCompaction()

# Remove old files no longer referenced
devices_table.vacuum() 
```