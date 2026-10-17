# PySpark & DBT Project

## Overview
This project implements the Medallion Architecture using PySpark and Databricks to process loan-related data through Bronze, Silver, and Gold layers.

## Architecture
- **Bronze Layer:** Ingests raw loan, loan schedule, and repayment CSV files into Delta tables using PySpark Structured Streaming.
- **Silver Layer:** Cleans, validates, and transforms raw data to improve data quality and consistency.
- **Gold Layer:** Creates business-ready datasets for reporting, analytics, and dashboard development.

## Technologies Used
- Azure Databricks
- PySpark
- DBT
- Apache Spark Structured Streaming
- Delta Lake
- Python
- GitHub

## Project Structure
```text
loan-data-engineering-project/
├── bronze/
│   ├── bronze_layer.ipynb
│   └── README.md
├── silver/
│   └── README.md
├── gold/
│   └── README.md
└── README.md
```

## Data Sources
The project uses three CSV datasets:
- `sch_loan` – Loan schedule data
- `Loan_data` – Loan account data
- `repayment_data` – Loan repayment data

## Workflow
1. Read raw CSV files from Databricks Volumes.
2. Infer the schema using PySpark batch reads.
3. Ingest data using Structured Streaming.
4. Store the ingested data in Delta tables in the Bronze layer.
5. Prepare the Silver layer for data cleansing and transformation.
6. Build Gold-layer datasets for business reporting and analytics.

## Objective
To build a scalable data engineering pipeline that transforms raw loan data into reliable, business-ready datasets using modern data engineering technologies.

## Project Status
- [x] Bronze Layer – Raw data ingestion
- [ ] Silver Layer – Data cleansing and transformation
- [ ] Gold Layer – Business-level aggregations and analytics

## Author
Sonali Gupta

*This project is developed for learning and portfolio purposes using sample data.*
