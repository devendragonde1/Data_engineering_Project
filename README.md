📊 File Comparison and Data Quality Framework 🔹 Overview

This project implements a data quality and validation framework to compare datasets, detect inconsistencies, and generate structured validation reports- It ensures reliable and high-quality data for downstream analytics.

🏗️ Architecture

The project follows the Medallion Architecture:
- Bronze Layer → Raw data ingestion from ADLS (CSV files)
- Silver Layer → Data cleaning and transformation
- Gold Layer → Data validation and reporting
  
⚙️ Tech Stack
- Azure Data Lake Storage Gen2 (ADLS)
- Azure Databricks
- PySpark
- Unity Catalog
- Databricks SQL Dashboard

📌 Key Features
File and dataset comparison across multiple sources
- Schema/column difference detection
- Row count validation
- Null value analysis
- Statistical comparison for data consistency
- Validation report generation
  
🔄 Workflow
- Ingest raw files into the Bronze layer
- Transform and clean data in the Silver layer
- Execute validation checks in the Gold layer
- Store results in a validation report table
- Visualize results using Databricks Dashboard

⚡ Pipeline Execution
- Implemented workflow orchestration using Databricks Jobs
- Automated execution of multiple notebooks in sequence
- Pipeline is manually triggered for execution
- Ensures consistent and repeatable data validation process

📊 Dashboard
- An interactive dashboard is created using Databricks SQL Dashboard to:
- Monitor validation results
- Analyze dataset differences
- Explore data quality metrics using filters

📊 Output
- The framework generates a structured report including:
- Dataset/File names
- Validation type
- Differences identified Data quality insights

🚀 Future Enhancement
- Schedule pipeline for automated execution
- Data quality scoring mechanism
- Alerting for validation failures
- Historical tracking of data quality
