# Wonderland Property Group (WPG) Cloud-Based Data Pipeline

This document details the design and implementation of a **cloud-based data pipeline** for **Wonderland Property Group (WPG)**, a real estate company dealing with diverse and scattered data.  
The project aims to build a **scalable and intelligent system on AWS** capable of handling real-time data and supporting predictive analytics using machine learning models.

---

##  Project Scope and Objectives

As a cloud data analyst, the goal was to create a system that can:

1. **Collect and Integrate Data**  
   - Gather structured, semi-structured, and unstructured data.  
   - Sources include smart homes (IoT), real estate transactions, customer behavior, and external research.

2. **Ensure Data Security and Compliance**  
   - Store data securely while adhering to **GDPR** and **CCPA** regulations.

3. **Enable Real-Time Analytics**  
   - Perform rapid analysis on instant transactions and sensor data.

4. **Develop Predictive Models**  
   - Use **AI/ML** to predict property values, classify customers, and provide personalized recommendations.

5. **Support Business Intelligence**  
   - Provide interactive reports and dashboards for managers and stakeholders.

---

##  Technical Architecture and Implementation

The solution is built on **AWS Cloud Infrastructure** with a layered data management approach.  

### 1. Data Ingestion
- Tools used: **Amazon AppFlow**, **AWS DMS**, **AWS IoT Core**, **Amazon Kinesis**  
- Collects data from various internal and external sources.

### 2. Storage and Processing
- **Data Lake on Amazon S3** with three zones:
  - Raw
  - Processed
  - Analytics
- **AWS Glue** for ETL operations.  
- **Amazon Lake Formation** for access control.

### 3. Analytics Layer
- **Amazon Athena**: Quick SQL queries on S3 data.  
- **Amazon Redshift**: Data warehouse for complex analysis.  
- **Amazon SageMaker**: Build and deploy machine learning models.

### 4. Security Layer
- **IAM**: Access management  
- **AWS KMS**: Encryption  
- **Amazon GuardDuty**: Threat detection

> Implementation includes Python scripts for IoT data simulation and Kinesis Firehose configuration, as well as a CloudFormation YAML template for automated resource deployment.

---

## Outcomes and Future Suggestions

- **Cost Reduction**: 25-30% compared to an on-premise setup.  
- **Scalable & Secure**: Provides a compliant cloud solution for WPG.  
- **Future Improvements**:
  - Strengthen real-time monitoring.  
  - Enhance security measures.  
  - Integrate additional data sources and resources.
