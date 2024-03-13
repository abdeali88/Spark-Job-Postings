# Real-time Job Posting Analytics

## Overview
The Real-time Job Posting Analytics project is designed to extract, process, and analyze job postings in real-time using Apache Spark on Docker. Leveraging scalable Spark clusters, the system processes streaming data from diverse sources, including unstructured text files and structured JSON files. The project implements regular expressions to extract key job information, achieving an impressive 98% data extraction success rate.

![System Architecture Diagram](/imgs/Architecture.png)

## Features
- **Data Extraction:** Utilizes Apache Spark to extract job information from both unstructured text files and structured JSON files.
- **Scalable Processing:** Leverages Spark clusters in Python for scalable and efficient processing of streaming data.
- **Cloud Storage:** Implements a scalable cloud storage solution on AWS using S3 to store parsed job information.
- **Data Management and Analysis:** Utilizes AWS Glue for data management and analysis, enabling real-time insights into job market trends.

## Screenshots
1. ![S3 Parquet Stream](/imgs/S3%20Streams.png)
2. ![Real Time Job Postings Data in Athena](/imgs/Athena%20Tables.png)

## Getting Started
To get started with the Real-time Job Posting Analytics project, follow these steps:
1. Clone the repository.
2. Set up Apache Spark on Docker.
3. Configure AWS S3 for storage and AWS Glue for data management.
4. Run the Spark job to start processing real-time job postings.
