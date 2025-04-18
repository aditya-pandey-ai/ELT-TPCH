# ELT-TPCH

This project implements an ELT (Extract, Load, Transform) pipeline using the TPCH dataset from Snowflake, orchestrated with Apache Airflow. It serves as a demonstration of building scalable data pipelines for analytical processing.

## Summary

This project includes a full end-to-end ELT pipeline with the following components:

1. **Snowflake RBAC Setup**  
   - Defined and managed Snowflake roles, warehouses, users, schemas, and databases to follow principle-of-least-privilege access.

2. **`dbt_project.yml` Configuration**  
   - Set up the DBT project structure including versioning, model paths, and materialization strategies.

3. **Staging and Sourcing Models**  
   - Created DBT models to source raw data and stage it into a clean, standardized format.

4. **Fact Tables and Data Marts**  
   - Built data marts and fact tables to enable analytics-ready datasets.

5. **DBT Macros**  
   - Wrote reusable Jinja macros for repetitive SQL logic and dynamic configurations.

6. **Generic and Singular Tests**  
   - Implemented data quality checks using DBT's generic tests and custom singular test cases.

7. **Orchestration Using Apache Airflow**  
   - Managed the entire ELT workflow using Airflow DAGs for task scheduling and monitoring.

## Project Overview

The ELT-TPCH project demonstrates extracting data from Snowflake's TPCH dataset, transforming it using DBT, and orchestrating the workflow with Apache Airflow. The project illustrates real-world data engineering best practices for enterprise-grade pipelines.

## Project Structure

- `dags/`: Airflow DAGs defining the ELT pipeline.  
- `tests/`: Unit and integration tests for Airflow tasks and DBT models.  
- `Dockerfile`: Docker image setup for the Airflow environment.  
- `.astro/`: Astronomer CLI configurations for local Airflow development.  
- `requirements.txt`: Python dependencies.  
- `packages.txt`: System-level package requirements.  
- `.gitignore`, `.dockerignore`: Ignored files during development and containerization.

## TPCH Dataset

The TPCH dataset is a standard benchmark for evaluating the performance of database systems. It simulates a business scenario involving orders, customers, and suppliers, providing a comprehensive dataset for testing data processing workflows.

## Preview
Below is a preview of the final output from the pipeline after data has been extracted, transformed, and loaded using DBT and orchestrated via Airflow:


The preview includes fact tables and transformed marts ready for analytical use.



## Contributing

Contributions are welcome! If you have suggestions for improvements or new features, feel free to fork the repository and submit a pull request.

## License

This project is licensed under the MIT License.

## Contact

For any inquiries or feedback, please reach out via linkedin.
