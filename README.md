Author: Md Nadeem Ansari  
Date: 15-09-2025  

# StreamStack | Realtime Data Engineering Pipeline  

## Table of Contents
- [Introduction](#introduction)
- [System Architecture](#system-architecture)
- [Key Takeaways](#key-takeaways)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)

## Introduction  

**StreamStack** is a complete end-to-end realtime data engineering project.  
The pipeline demonstrates how raw data can be ingested, processed, and stored using modern distributed technologies.  

It showcases how to:  
- Ingest live data streams,  
- Orchestrate and monitor workflows,  
- Process data at scale with distributed systems,  
- Store the results in reliable databases,  
- All containerized using Docker for seamless deployment.  

This project is designed to give learners and practitioners a **hands-on experience** with production-grade data engineering workflows.  

## System Architecture  

![System Architecture](./Data%20engineering%20architecture.png)  

The pipeline consists of the following layers:  

- **Data Source** → Generates realtime data using the `randomuser.me` API.  
- **Apache Airflow** → Orchestrates the pipeline, fetching data and storing raw records in PostgreSQL.  
- **Apache Kafka + Zookeeper** → Streams data from PostgreSQL into a distributed processing system.  
- **Schema Registry & Control Center** → Manages Kafka schemas and provides monitoring capabilities.  
- **Apache Spark** → Performs distributed data processing at scale.  
- **Cassandra** → Stores the final transformed data.  

## Key Takeaways  

By building StreamStack, you will learn:  

- How to set up an **end-to-end realtime pipeline**  
- Using **Apache Airflow** for scheduling and orchestration  
- Implementing **Apache Kafka** for scalable data streaming  
- Managing **distributed coordination** with Zookeeper  
- Processing data using **Apache Spark (cluster mode)**  
- Persisting data into **Cassandra and PostgreSQL**  
- Running everything in **Docker containers**  

## Tech Stack  

- Python  
- Apache Airflow  
- Apache Kafka  
- Apache Zookeeper  
- Apache Spark  
- Cassandra  
- PostgreSQL  
- Docker  

## Getting Started  

1. Clone the repository:  
    ```bash
    git clone https://github.com/N-ansari1902/streamstack.git
    ```

2. Navigate to the project folder:  
    ```bash
    cd streamstack
    ```

3. Start the services with Docker Compose:  
    ```bash
    docker-compose up
    ```

That’s it — your realtime data engineering pipeline is live! 🎉  

---
