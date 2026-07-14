# Walmart Data Engineering Pipeline

## About the Project

This project is an end-to-end Data Engineering pipeline built using Apache Airflow, AWS S3, Databricks, dbt, Docker, Python, and SQL.

The objective of this project is to automate the complete data pipeline, starting from loading raw CSV files into AWS S3 to transforming them into analytics-ready tables using the Medallion Architecture (Bronze, Silver, and Gold layers).

While working on this project, I learned how different data engineering tools work together to build scalable and automated data pipelines. It also helped me gain practical experience with workflow orchestration, data transformation, data quality testing, snapshots, and dimensional data modeling.

---

## Technologies Used

- Apache Airflow
- Docker
- AWS S3
- Databricks
- dbt (Data Build Tool)
- Python
- SQL
- Git
- GitHub

---

## Project Workflow

The pipeline follows the following steps:

1. Raw CSV files are uploaded to AWS S3.
2. Apache Airflow triggers the complete workflow.
3. Databricks loads the raw data into the Bronze layer.
4. dbt transforms the data into the Silver Technical layer.
5. Data quality tests are executed using dbt.
6. Business-ready models are created in the Silver Business layer.
7. Fact and Dimension tables are generated in the Gold layer.
8. Snapshots are used to maintain historical records of changing data.

---

## Features

- Automated end-to-end data pipeline
- Workflow orchestration using Apache Airflow
- Data ingestion from AWS S3
- Data transformation using dbt
- Bronze, Silver and Gold architecture
- Data quality validation
- Source freshness checks
- Snapshot implementation
- Fact and Dimension data modeling
- Docker-based development environment
- Version control using Git and GitHub

---

## Project Structure

```text
airflow_dbt_project/

├── dags/
├── config/
├── walmart_project/
│   ├── models/
│   ├── snapshots/
│   ├── macros/
│   ├── tests/
│   └── sources/
├── Dockerfile
├── docker-compose.yml
├── requirements.txt
└── README.md
```

---

## Architecture

```
CSV Files
     │
     ▼
AWS S3
     │
     ▼
Apache Airflow
     │
     ▼
Databricks
     │
     ▼
Bronze Layer
     │
     ▼
Silver Technical Layer
     │
     ▼
Silver Business Layer
     │
     ▼
Gold Layer
(Fact and Dimension Tables)
```

---

## Screenshots

The following screenshots demonstrate different stages of the project:

- Airflow DAG
- Successful Airflow Pipeline Execution
- AWS S3 Bucket
- Databricks Catalog and Tables
- dbt Lineage Graph

(Add the screenshots here.)

---

## What I Learned

Through this project, I gained practical experience with:

- Building end-to-end data pipelines
- Workflow orchestration using Apache Airflow
- Using Docker for project setup
- Data ingestion using AWS S3
- Data transformation using dbt
- Medallion Architecture
- Data quality testing
- Snapshot implementation
- Fact and Dimension modeling
- Git and GitHub workflow

---

## Future Improvements

Some improvements that can be added in the future include:

- CI/CD using GitHub Actions
- Monitoring and alerting for pipeline failures
- Integration with BI tools for reporting
- Deployment on cloud infrastructure
- Support for larger datasets

---

## Author

Kanishka Verma

B.Tech Computer Science Engineering (AI & ML)

Aspiring Data Engineer

