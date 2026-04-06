4 product lines

Lakeflow - ETL and ingestion
  - connect - easily connect data sources
  - DLT - reliable pipelines 
  - Jobs - scheduling and triggering of processes to run your data ingestion or transformation workflows.
SQL Warehousing - storage and structure
  - a data warehousing product 
  - data and unity catalog
  - automatic tooling for migrating from other data stores to Databricks SQL
AI & BI - 
  - provides an assistant called AI/BI Genie - LLM for helping build dashboards and exploring data
Mosaic AI
  - suite of tools for traditional AI application development
  - focus on genAI applications
  - ML Flow & AutoML

Common challenges to data engineers
- complex lakeflow connect workflows
- isolating dev environments and prod environments

Lakflow Overview
- getting data into the platform
- 3 components
  - Connect
    - Efficient, no-code connectors. i.e. Salesforce, Google Analytics, Meta, etc.
    - extracts data to databases
  - DLT
    - supports medallion

  - Jobs
    - serverless job execution
    - scaleable, event driven

Delta Lake Overview
- data ingestion arrives into delta lake
- use delta tables in delta lake
- data is stored as parquet files + transaction logs which are stored as JSON
- delta adds a transaction (log file) and the actual structured data (parquet)

Learn about
- ACID Transactions - atomicity, consistency, isolation, durability
- DML Operations - Data Manipulation Language - INSERT, UPDATE, DELETE, MERGE
- Time travel - 
- Schema Evolution & Enforcement - automatically adjust the schema of DLT, ensures all data conforms to the specified schema

- `CREATE TABLE __table_name__ AS` - this statement allows us to create tables from data sources that are unconventional to standard SQL
- `COPY INTO` - this statement allows us to modify an existing table with an enforced schema
- 

Medallion Architecture
- Bronze: Dumping ground for raw data from external sources
  - Long retention period
  - Data in it's original format
- Silver: Structured and schema enforced
  - Filter, cleanse, join, enrich
  - define the structure
  - evolve the schema at this point
- Gold: Clean data, ready for consumption
  - Business-level aggregates
  - Delivered downstream for users

Data pipelines are usually very complex. They will often have a bronze dedicated to a single data source. Then multiple silvers which hold the different split-out, aggregated, and schema enforced data. Finally, gold tables will hold the data in it's most ready to use state.






