# pyspark-github-events
Build a production-style batch data pipeline using Apache Spark to process GitHub event logs


For [dataskew.io](https://dataskew.io/projects/batch-processing-spark) project.

```
github-analytics/
├── docker/
│   └── spark/               # Dockerfile for Spark runtime
├── data/
│   ├── raw/                 # GitHub Archive .json.gz files
│   └── output/              # Partitioned Parquet output
├── jobs/
│   ├── ingest.py            # Read and normalize raw JSON
│   ├── transform.py         # Filter, clean, enrich with derived columns
│   ├── aggregate.py         # Compute KPIs and metrics
├── config/
│   └── job_config.yaml      # Input/output paths, date ranges, etc.
├── scripts/
│   └── run_job.sh           # CLI wrapper for spark-submit
├── tests/                   # Unit tests for logic and edge cases
├── requirements.txt
└── README.md
```
