**Context:** You need an exact copy of a dataset in a different environment (e.g., Prod to Staging) for testing or redundancy, often involving non-idempotent sources.

**Solution:** A simple Extract-Load (EL) job that copies data without modification. Can be code-based or infrastructure-based (e.g., S3 Replication). Ideally utilizes "Push" semantics to avoid impacting the source environment's stability.

**Challenges:**

- **Metadata:** Ensure file attributes, headers, and ordering (e.g., Kafka offsets) are preserved.
    
- **Isolation:** Use push replication to prevent the destination environment from starving source resources.
    

**Code Example (Python/Spark - Raw Copy):**

Python

```
# Read as raw text to avoid schema inference/corruption
input_dataset = spark_session.read.text(f'{base_dir}/input/date=2023-11-01')
input_dataset.write.mode('overwrite').text(f'{base_dir}/output-raw/date=2023-11-01')
```

---

### 5. Transformation Replicator

**Context:** You need to replicate production data to lower environments (Staging/Dev) but must remove PII (Personally Identifiable Information) or sensitive fields.

**Solution:** Add a transformation step between Extract and Load. This can involve dropping columns, masking values, or filtering rows.

**Challenges:**

- **Schema Drift:** Silent transformations (like date formatting) can break downstream tests.
    
- **Desynchronization:** Privacy rules change; relying on manual logic can lead to leaks. Use governance tools/tags where possible.
    

**Code Example (Python/Spark - Dropping Columns):**

Python

```
input_delta_dataset = spark_session.read.format('delta').load(users_table_path)

# Remove PII columns
users_no_pii = input_delta_dataset.drop('ip', 'latitude', 'longitude')

# Masking a column
from pyspark.sql import functions as F
devices_trunc = input_delta_dataset.withColumn(
    'full_name', 
    F.expr('SUBSTRING(full_name, 2, LENGTH(full_name))')
)
```