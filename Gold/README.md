# Gold Layer – Loan Data Engineering

## Overview
The Gold layer transforms Silver-layer loan, repayment, and loan schedule data into business-ready datasets for loan collection and repayment analysis.

## Objectives
- Generate loan-level collection summaries.
- Analyze monthly repayments.
- Prepare aggregated datasets for reporting and business insights.
- Store curated data in Delta tables.

## Data Sources
The Gold layer uses cleaned data from the Silver layer:
- `loan_data`
- `repayment_data`
- `sch_loan`

## Transformations
- Join loan, repayment, and loan schedule datasets.
- Select relevant business columns.
- Calculate loan-wise collection metrics.
- Aggregate repayment amounts for monthly analysis.
- Prepare datasets for downstream reporting.

## Gold Tables
| Table | Purpose |
|---|---|
| `collection_summary` | Loan collection summary |
| `month_repayment` | Monthly repayment analysis |

## Technology Stack
- Azure Databricks
- PySpark
- Delta Lake
- SQL
- Unity Catalog
- Databricks Workflows

## Pipeline Flow
**Bronze → Silver → Gold**

- **Bronze:** Streaming ingestion of raw data.
- **Silver:** Data cleaning, validation, deduplication, and upserts.
- **Gold:** Business-ready loan collection and repayment datasets.

## Output
The Gold tables can be used for SQL analysis, dashboards, and business reporting.

## Key Learning
This project demonstrates multi-layer data processing, PySpark joins and aggregations, Delta table management, and workflow orchestration using Databricks.

---
*Part of my hands-on Data Engineering project focused on building a loan data pipeline using Azure Databricks and PySpark.*
