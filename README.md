# RFM-Based Customer Segmentation with KMeans-Clustering

This project focuses on customer segmentation based on Recency, Frequency, and Monetary (RFM) analysis using K-Means clustering. The goal is to identify distinct customer segments and tailor strategies accordingly to enhance customer satisfaction and business outcomes.

## Project Overview

### Architecture

![Project Architecture](Project%20Architecture.jpg)

1. **Data Sources:** The raw data is sourced from multiple databases and is uploaded to AWS S3.
2. **AWS S3 Bucket:** The data is stored in structured folders within the AWS S3 bucket.
3. **Databricks:** 
   - **Exploratory Data Analysis (EDA):** Data is fetched from S3 and cleaned using Apache Spark.
   - **RFM Modeling:** RFM values are calculated to determine customer value.
   - **K-Means Clustering:** The RFM values are segmented into different customer clusters.
   - **SQL Queries:** Further analysis and data extraction are performed using SQL.
4. **Tableau:** The final clustered data is visualized using Tableau for actionable insights.
5. **Local Storage:** Visualizations and reports are stored locally for easy access.

## Project Workflow

1. **Data Ingestion:** Raw data is uploaded to an AWS S3 bucket.
2. **Data Cleaning & Preprocessing:** Data is cleaned and preprocessed using PySpark on Databricks.
3. **RFM Analysis:** 
   - Calculate Recency, Frequency, and Monetary values.
   - Remove outliers and filter the dataset to focus on key regions (e.g., United Kingdom).
4. **K-Means Clustering:** Apply K-Means clustering on RFM values to segment customers into distinct groups.
5. **Data Analysis:** Run SQL queries on the clustered data for deeper insights.
6. **Visualization:** Use Tableau to create visualizations based on the final clustered data.
7. **Reporting:** Save the visualizations and insights to local storage for reporting.
