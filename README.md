# Real-Time - DataStreaming
# Real-Time Data Streaming and Processing Pipeline

## Overview

This project showcases an end-to-end data engineering pipeline, demonstrating how to handle real-time data ingestion, processing, and storage. The pipeline integrates multiple technologies, including Apache Airflow, Apache Kafka, Apache Zookeeper, Apache Spark, Cassandra, and Docker, to ensure seamless data flow and processing.

The pipeline begins by fetching synthetic user data from the `randomuser.me` API. This raw data is orchestrated and stored in a **PostgreSQL** database using **Apache Airflow**. To enable real-time data streaming, **Apache Kafka** and **Apache Zookeeper** are used to stream data from PostgreSQL to the processing engine. The **Control Center** and **Schema Registry** provide schema management and monitoring capabilities for the Kafka streams.

**Apache Spark** processes the streamed data, transforming and preparing it for storage. The processed data is then stored in a **Cassandra** database, ensuring efficient and scalable data storage. The entire pipeline is containerized using **Docker**, facilitating easy deployment and management across different environments.

### Prerequisites
- Docker
- Docker Compose
- Python
- Apache Airflow
- Apache Kafka
- Apache Zookeeper
- Apache Spark
- Cassandra
- PostgreSQL

## Architecture Diagram
![Data Flowchart](https://github.com/user-attachments/assets/2c84da9f-8728-4e93-9a5e-26a5e3f084a0)

## Technologies Used
- **Data Source**: `randomuser.me` API for generating random user data.
- **Apache Airflow**: Orchestrates the pipeline and stores data in PostgreSQL.
- **Apache Kafka** and **Zookeeper**: Streams data from PostgreSQL to the processing engine.
- **Control Center** and **Schema Registry**: Manages schemas and monitors Kafka streams.
- **Apache Spark**: Processes data using master and worker nodes.
- **Cassandra**: Stores the processed data.
- **Docker**: Containerizes the entire pipeline for portability and scalability.

## Learning Outcomes
- Setting up a data pipeline with **Apache Airflow** for workflow orchestration.
- Implementing real-time data streaming with **Apache Kafka**.
- Managing distributed synchronization with **Apache Zookeeper**.
- Applying data processing techniques using **Apache Spark**.
- Storing and managing data using **PostgreSQL** and **Cassandra**.
- Containerizing the data engineering infrastructure with **Docker** for seamless deployment.

### Usage
- Access the Airflow web interface at `http://localhost:8080` to monitor and manage the pipeline.
- Use the Control Center and Schema Registry to manage Kafka streams.
- Query processed data from Cassandra for analysis and reporting.

## Conclusion
This project provides a robust framework for real-time data streaming and processing, leveraging a combination of powerful tools and technologies to create an efficient and scalable data engineering pipeline. By following this guide, you will gain hands-on experience with setting up and managing complex data workflows, preparing you for real-world data engineering challenges.

## Acknowledgements
Special thanks to [Yusuf Ganiyu](https://www.linkedin.com/in/yusuf-ganiyu-b90140107/) for the inspiration and guidance on this project.
