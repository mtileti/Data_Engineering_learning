# AWS S3 and Athena Data Lake Project

## Overview

This project demonstrates how to build a simple serverless data lake architecture using **Amazon S3** and **Amazon Athena** for querying and analyzing data. All services used are fully managed and serverless, eliminating the need for infrastructure provisioning.

## AWS Services Used

- **Amazon S3**: Scalable object storage used as a data lake.
- **Amazon Athena**: Serverless query service used to analyze structured data stored in S3 using SQL.

## Steps Performed

### 1. Amazon S3 Setup
- Created a new S3 bucket to store all raw data and query results.
- Inside the bucket:
  - Created a folder named `input/` to store raw CSV/JSON files.
  - Created a folder named `query-results/` to store the output of Athena queries.
- Copied the S3 path for the query results and configured it in Athena settings.

### 2. Amazon Athena Configuration
- Athena was used as a **serverless ETL tool** to perform SQL queries directly on data stored in S3.
- Created a new database: `trendytech_db`.
- Defined an external table in Athena pointing to the input file in S3.
- Specified the schema during table creation (columns, data types, etc.).
- Ran SQL queries on the external table to analyze data.
- Note: AWS charges **$5 per TB scanned** in Athena.

## Output
- Query results were successfully written to the designated S3 folder.
- Sample analysis was completed using SQL in Athena.

## Conclusion
This project showcases how easy and cost-effective it is to build a serverless data lake using Amazon S3 and Athena. It is ideal for ad-hoc querying, quick data exploration, and lightweight ETL tasks without managing any infrastructure.

---

## Author
Madhusudhan Tilleti

