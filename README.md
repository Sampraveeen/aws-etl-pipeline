# AWS ETL Data Pipeline using Python, S3, EC2 and RDS PostgreSQL

Developed by: Samiksha P  
Sri Manakula Vinayagar Engineering College, Puducherry  

---

## Project Overview

This project demonstrates a complete ETL (Extract, Transform, Load) data pipeline built on AWS Cloud.  
The main goal is to extract data from an S3 bucket, perform basic transformations using Python and Pandas on an EC2 instance, and then load the cleaned data into an Amazon RDS PostgreSQL database.

The project helped me understand how AWS services like S3, EC2, RDS, and IAM can be combined together to automate data handling and transformation in a real-time cloud environment.

---

## AWS Services Used

1. **Amazon S3** – To store input data files (e.g., data.csv)
2. **Amazon EC2** – To host and run the Python ETL script
3. **Amazon RDS (PostgreSQL)** – To store the processed and transformed data
4. **IAM** – To securely manage AWS access keys and permissions
5. **Security Groups** – To control inbound and outbound network access

---

## How It Works

1. Upload the raw CSV file to an S3 bucket (example: `etl-data-bucket-samiksha`).
2. The EC2 instance connects to S3 using `boto3` and downloads the file.
3. The Python script transforms the data (e.g., converts height from inches to centimeters).
4. The transformed data is then uploaded into a PostgreSQL table on Amazon RDS.
5. The process completes with confirmation messages for each stage.

---

## Technologies Used

- Python 3  
- Pandas  
- Boto3  
- Psycopg2  
- AWS EC2  
- AWS S3  
- AWS RDS (PostgreSQL)  
- Ubuntu 24.04 (as EC2 instance OS)

---

## Folder Structure

AWS_ETL_Pipeline  
│  
├── etl_script.py (Main ETL Python script)  
├── requirements.txt (Dependencies file)  
├── data.csv (Sample dataset)  
└── README.md (Project documentation)

---

## Example Input (data.csv)

name,height_in  
Alice,60  
Bob,70  
Charlie,65  

---

## Example Console Output

Extracting data from S3...  
Data extracted successfully.  
Transforming data...  
Data transformed successfully.  
Loading data into PostgreSQL...  
Data loaded successfully.  

---

## What I Learned

Through this project, I learned how to:
- Connect EC2, S3, and RDS seamlessly in a single workflow  
- Use IAM credentials and security groups securely  
- Perform data transformation using Pandas  
- Load transformed data into PostgreSQL using Psycopg2  
- Manage cloud resources and troubleshoot access or connection issues  

This project gave me a clear understanding of how ETL pipelines operate in cloud-based environments.

---

## Future Improvements

- Automate the ETL process using AWS Lambda and EventBridge  
- Add error handling and logging using AWS CloudWatch  
- Perform complex transformations on larger datasets  
- Build a small monitoring dashboard for data updates  

---

## About

This project was part of my academic cloud and AI implementation tasks,  
focusing on integrating data and machine learning readiness within cloud services.

GitHub Repository: [https://github.com/Sampraveeen](https://github.com/Sampraveeen)

---

*This repository was created purely for learning and demonstration purposes.*
