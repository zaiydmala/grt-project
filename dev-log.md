## 28-01-2026

**Work Done**
- Created resource group
- Created ADLS with containers

## 30-01-2026

**Work Done**
- create 2 linked services
  - adls connection
  - gtfs connection
-  create 2 datasets
  - gtfs source
  - gtfs sink
- run pipeline
- create databricks workspace
- create databricks service principal and give rbac of blob contributor and change spark configs
- create a notebook to unzip latest zip files from raw and send to bronze
- create bronze_to_delta.py to make data queryable

## 02-02-2026

**Work Done**
- create 01_bronze_gtfs_ingest.py that creates delta tables of the extracted files
- remember that we service principal authenticated databricks with adls
- remember python dictionery comprehension
- run validation
  - loop through each delta table and check rows
  - check row count
  - look at schema
