**Context:** Downstream jobs need to know exactly when a dataset is complete to avoid processing partial data.

**Solution:** Create a specific signal file (e.g., `_SUCCESS`) or use a partition convention (consumers wait for partition `N+1` before processing `N`).

**Challenges:**

- **Enforcement:** It is often a convention, not a hard lock. Consumers might ignore the marker and read partial data.
- **Late Data:** If data arrives after the marker is written, the partition might need to be re-opened/re-processed.

**Python/Airflow - FileSensor**

```python
from airflow.sensors.filesystem import FileSensor

# Wait for the _SUCCESS file to appear
wait_for_data = FileSensor(
    task_id='wait_for_data',
    filepath=f'{input_data_file_path}/_SUCCESS',
    mode='reschedule' # Release worker slot while waiting
)
```

**Python/Airflow - Creating Marker**

```python
@task
def create_readiness_file():
    with open(f'{dataset_dir}/COMPLETED', 'w') as marker_file:
        marker_file.write('')
```