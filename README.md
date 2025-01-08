# Stock Market Kafka Real-Time Data Engineering Project

## Introduction
This project demonstrates an **End-to-End Data Engineering pipeline** for processing and analyzing **real-time stock market data** using Apache Kafka and AWS services. The focus is on building a scalable and efficient pipeline that integrates various tools and technologies for producing, storing, and querying real-time data.

---

## Objective
The primary objective is to process stock market data in real-time using a **Kafka producer** and **consumer** setup, store the data in **Amazon S3**, and analyze it using **AWS Glue** and **Athena**.

---

## Architecture Workflow
1. **Data Simulation**: A Python-based stock market application simulates data and produces it using Apache Kafka.
2. **Producer**: Kafka produces the simulated stock market data and sends it to a topic.
3. **Consumer**: Kafka consumers retrieve data and store it in Amazon S3.
4. **Storage**: Data is stored in an S3 bucket for further processing.
5. **Data Crawling**: AWS Glue Crawler scans the S3 bucket to create a Glue Data Catalog.
6. **Querying and Analysis**: Athena is used to query and analyze the data in the Glue Catalog.

### Architectural Diagram
![Architecture Diagram](workflow.jpg)

---

## Technology Stack
- **Programming Language**: Python
- **Data Processing**: Apache Kafka
- **Cloud Services**: 
  - **S3**: For data storage
  - **AWS Glue Crawler**: For creating a metadata catalog
  - **AWS Glue Data Catalog**: For managing metadata
  - **Amazon Athena**: For querying and analyzing data
  - **EC2**: For hosting Kafka and running producers/consumers
