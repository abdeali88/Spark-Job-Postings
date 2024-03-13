# Real-time Job Posting Analytics

## Overview
The Real-time Job Posting Analytics project is a sophisticated system developed to extract, process, and analyze job postings in real-time using **Apache Spark** on **Docker**. Traditional job posting data often comes in various formats and structures, making parsing and extracting relevant information a challenging task. This project tackles this challenge by employing **regular expressions** to identify patterns within the 650 job postings, enabling the extraction of key information such as job titles, descriptions, salary, dates, qualifications, and skills.

![System Architecture Diagram](/imgs/Architecture.png)

## Features
- **Data Extraction:**  Utilizes Apache Spark and regular expressions to parse job postings from both unstructured text files and structured JSON files. Extracted fields include job title, company name, location, salary range, required qualifications, and desired skills.
- **Scalable Processing:** Leverages Spark clusters in Python for efficient processing of streaming data. The system can handle large volumes of job postings with ease, ensuring real-time insights into job market trends.
- **Cloud Storage:**  Implements a scalable cloud storage solution on AWS using S3 to store parsed job information. Parquet files are written into the S3 bucket, enabling efficient storage and retrieval of data.
- **Data Management and Analysis:** Utilizes AWS Glue for data management and analysis, facilitating the creation of a structured database schema for the parsed job postings. With Athena, stakeholders can query and analyze the data in real-time, gaining valuable insights into job market dynamics.

## Extracted Fields from Job Description
- **Job Title**: The title of the job position being offered.
- **Company Name**: The name of the company offering the job.
- **Location**: The geographical location of the job.
- **Salary Range**: The range of salary offered for the job position.
- **Required Qualifications**: The qualifications and educational background required for the job.
- **Desired Skills**: The skills and experience desired by the employer for the job position.
- **Start and End Date**: The start and end date for the job application.


## Screenshots
### 1. Text File Job Description
![Text File Job Description](/imgs/TXT%20JD.png)

### 2. JSON File Job Description
![JSON File Job Description](/imgs/JSON%20JD.png)

### 3. S3 Parquet Streams
![S3 Parquet Stream](/imgs/S3%20Streams.png)

### 4. Job Postings Data in Athena
![Real Time Job Postings Data in Athena](/imgs/Athena%20Tables.png)

## Getting Started
To get started with the Real-time Job Posting Analytics project, follow these steps:
1. Clone the repository.
2. Set up Apache Spark on Docker.
3. Configure AWS S3 for storage and AWS Glue for data management.
4. Run the Spark job to start processing real-time job postings.
