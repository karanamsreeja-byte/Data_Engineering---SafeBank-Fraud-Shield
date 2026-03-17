# SafeBank Fraud Shield – Data Engineering Capstone

## Overview

SafeBank Fraud Shield is a scalable fraud detection data pipeline designed to detect suspicious financial transactions in near real-time.

The project implements a modern lakehouse architecture using Databricks and Delta Lake with Bronze, Silver, Gold, and Production layers.

The system processes millions of transactions and generates analytics dashboards for fraud monitoring.

---

## Architecture

Bronze → Silver → Gold → Production

Bronze Layer
- Raw ingestion of transaction data
- JSON transfer logs
- CSV account metadata
- Geo-IP lookup dataset

Silver Layer
- Data validation
- Geospatial enrichment
- Velocity tracking (transactions per hour)
- CDC merge for account balances

Gold Layer
- Fraud detection rules
- Risk score calculation
- Fraud alert generation
- Aggregated risk scoring

Production Layer
- Broadcast join optimization
- Delta optimization
- Z-order indexing
- PII masking
- Monitoring and logging

---

## Technologies Used

- Databricks
- Apache Spark
- Delta Lake
- SQL
- Python (PySpark)
- Git
- Dashboard Visualization

---

## Data Pipeline

1. Bronze Layer Ingestion
2. Silver Layer Transformation
3. Gold Layer Fraud Detection
4. Production Layer Optimization
5. Dashboard Analytics

Pipeline orchestration is handled using a Databricks job.

---

## Dashboard

Fraud Control Center dashboard provides:

- Fraud alerts by country
- Fraud alerts over time
- High-risk account monitoring
- Fraud distribution by risk level
- Average fraud transaction value

---

## Data Scale

Dataset size simulated:

5 Million+ transactions

Designed to scale to production workloads.

---

## Job Automation

Pipeline is automated using Databricks Jobs with scheduled execution.

Example schedule:
Every 1 hour.

---

## Security

PII masking applied to sensitive fields:

- Account identifiers
- Customer names

---

## Validation

Data validation rules implemented to detect malformed records and ensure data quality.

---

## Repository Structure

notebooks/
dashboards/
validation/
architecture/
data_samples/

---

## Author

Karanam Sree
Data Engineering Capstone Project