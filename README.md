# Wonderland Property Group — Cloud Data Pipeline Architecture

An AWS cloud architecture design for a real estate company (Wonderland Property Group) handling scattered, multi-source data — covering data ingestion, storage, real-time analytics, machine learning, and security.

> **Note:** This is an architecture and system design document (see the full PDF report), not a deployed or coded implementation. It demonstrates the ability to design a cloud data platform from requirements to component selection.

## Objectives

The design addresses five goals:
1. **Data Integration** — collect structured, semi-structured, and unstructured data from IoT smart-home sensors, real estate transactions, customer behavior, and external research
2. **Security & Compliance** — GDPR and CCPA-compliant data storage
3. **Real-Time Analytics** — rapid analysis of live transactions and sensor data
4. **Predictive Modeling** — ML-based property valuation, customer classification, and recommendations
5. **Business Intelligence** — interactive dashboards for stakeholders

## Architecture

| Layer | AWS Services |
|---|---|
| **Ingestion** | Amazon AppFlow, AWS DMS, AWS IoT Core, Amazon Kinesis |
| **Storage & Processing** | Amazon S3 (Raw / Processed / Analytics zones), AWS Glue (ETL), Amazon Lake Formation |
| **Analytics** | Amazon Athena (SQL queries), Amazon Redshift (data warehouse), Amazon SageMaker (ML) |
| **Security** | IAM, AWS KMS (encryption), Amazon GuardDuty (threat detection) |

## Projected Outcomes

- 25–30% cost reduction vs. an on-premise setup
- Scalable, GDPR/CCPA-compliant cloud infrastructure

## Future Work

- Strengthen real-time monitoring
- Enhance security measures
- Integrate additional data sources

## Full Report

See [Real-Time Data Integration and Analytics in Real Estate Using AWS Cloud Services.pdf](<Real-Time Data Integration and Analytics in Real Estate Using AWS Cloud Services.pdf>) for the complete design document.
