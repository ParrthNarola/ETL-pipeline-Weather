# ETL Weather Project

A data engineering project that extracts weather data from the Open-Meteo API, transforms it, and loads it into a PostgreSQL database using Apache Airflow.

## 🌤️ Project Overview

This project implements an ETL (Extract, Transform, Load) pipeline that:

- **Extracts** current weather data from the Open-Meteo API for London (51.5074°N, 0.1278°W)
- **Transforms** the raw API response into a structured format
- **Loads** the processed data into a PostgreSQL database for analysis and storage


## 🛠️ Tech Stack

- **Apache Airflow** - Workflow orchestration and scheduling
- **PostgreSQL** - Relational database for data storage
- **Open-Meteo API** - Weather data source
- **Docker** - Containerization platform
- **Python** - Programming language for ETL logic
- **Astro Runtime** - Airflow runtime environment
- **HTTP Hooks** - API integration
- **PostgreSQL Hooks** - Database connectivity

## 📁 Project Structure

```
ETL Weather/
├── dags/
│   ├── etlweather.py          # Main weather ETL pipeline
│   └── exampledag.py          # Example astronaut ETL DAG
├── docker-compose.yml         # PostgreSQL service configuration
├── Dockerfile                 # Airflow runtime configuration
├── requirements.txt           # Python dependencies
├── include/                   # Additional files
├── plugins/                   # Airflow plugins
└── tests/                     # Test files
    └── dags/
        └── test_dag_example.py
```
