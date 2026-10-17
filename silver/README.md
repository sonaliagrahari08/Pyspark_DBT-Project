📌 Project Overview

The Silver Layer is responsible for cleaning, validating, and transforming raw data ingested into the Bronze Layer. This project uses PySpark and Delta Lake in Azure Databricks to prepare reliable, structured data for downstream analytics.

🎯 Objectives

Clean and transform Bronze Layer datasets.

Perform data profiling and quality checks.

Remove duplicate records using business keys.

Retain the latest record based on the source CDC column, when available.

Add processing timestamps for auditing.

Implement incremental insert and update operations using Delta Lake MERGE.

Store cleansed data in Silver Delta tables.
