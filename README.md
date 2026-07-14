# Walmart Data Engineering End-to-End Project

This project is my attempt to build a complete data engineering pipeline using modern tools like Databricks, dbt, Apache Airflow and AWS S3.

The main goal of this project was to understand how data moves from different sources, gets transformed, validated, and finally becomes ready for analytics through an automated workflow.

---

## Project Architecture

<img width="1692" height="929" alt="architecture" src="https://github.com/user-attachments/assets/bf7be654-aff5-4323-b92d-0a7a83c9cb74" />

---

## About the Project

The pipeline starts by collecting data from two different sources.

- An **Agentic PostgreSQL Database**, where Change Data Capture (CDC) is used to capture database changes.
- **AWS S3**, which stores raw files for ingestion.

The data is then loaded into **Databricks**, where incremental processing is performed. Using **dbt**, the data is transformed into clean and structured models while running data quality checks at every important stage.

Finally, **Apache Airflow** orchestrates the complete workflow, making sure every step runs in the correct order automatically.

---

## Tech Stack

- Python
- SQL
- Databricks
- dbt
- Apache Airflow
- PostgreSQL
- AWS S3
- Change Data Capture (CDC)
- Docker
- Git & GitHub
- VS Code
- Ghost AI (used as a development assistant)

---

## Workflow

1. Capture data changes from the Agentic PostgreSQL Database using CDC.
2. Load raw files from AWS S3.
3. Perform incremental data ingestion in Databricks.
4. Transform the data using dbt.
5. Run automated data quality tests.
6. Build Silver and Gold data models.
7. Orchestrate the complete pipeline using Apache Airflow.

---

## Project Structure

```text
airflow/
│── dags/
│── plugins/
│── docker-compose.yaml
│── Dockerfile

walmart_project/
│── models/
│── snapshots/
│── tests/
│── macros/
│── seeds/
│── profiles.yml
```

---

## Screenshots

### Project Architecture

<img width="1692" height="929" alt="architecture" src="https://github.com/user-attachments/assets/30a9b704-f047-4c8b-b630-511afa8d1d7e" />

### Airflow DAG

<img width="1708" height="947" alt="airflow-dag" src="https://github.com/user-attachments/assets/f8955e79-8206-4183-b60a-7d790d8a27ee" />

### Databricks Job

<img width="1710" height="949" alt="databricks-job" src="https://github.com/user-attachments/assets/0e83b46b-8058-4891-9949-6fd00eec70a5" />


---

## What I Learned

Working on this project helped me understand how different tools in a modern data engineering stack work together.

I learned how to build an automated data pipeline, perform incremental data loading, work with CDC, transform data using dbt, validate data quality through tests, and orchestrate everything using Apache Airflow. It also gave me hands-on experience with Docker, Databricks, AWS S3, PostgreSQL and Git.

---

## Future Improvements

- Deploy the pipeline on cloud infrastructure.
- Add monitoring and alerting.
- Build dashboards for analytics.

---

If you have any suggestions or feedback, feel free to connect with me.
