# Databricks-Volumes-ETL-Pipeline-with-Azure-Integration
Architecture
Bronze → Silver (Valid / Bad / Processed) → Gold

Features

Incremental data ingestion using MERGE INTO

Validation with business rules and SQL lookups

Enrichment using product, customer, and store data

Advanced transformations (NetAmount, Margin)

Aggregations: sales, margin, top customers

End-to-end orchestration via Lakeflow Jobs

Notebooks

ingestion.py – reads & merges raw data into Bronze

validation.py – applies rules, splits valid/bad records

transformation.py – enriches and computes business metrics

aggregation.py – performs analytical aggregations

lakeflow_job – orchestrates the pipeline

Integrations

Azure SQL Database for lookup validation

Azure Key Vault for credential management

ADF for lookup ingestion into SQL
