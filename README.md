# 🚕 End-to-End Real-Time Analytics with Azure Synapse: NYC Taxi Trips Project

This project demonstrates an **end-to-end big data and analytics pipeline** using **Azure Synapse Analytics**, powered by **real-world NYC Taxi Trip data**. The solution ingests raw data, transforms it using **Serverless SQL and Spark Pools**, stores curated datasets in **Dedicated SQL Pools**, and serves interactive reports via **Power BI** — all orchestrated through **Synapse Pipelines**.

> 📍 This project reflects a real-world use case and enterprise-grade architecture. It's built for recruiters, hiring managers, and tech leads to evaluate my hands-on expertise in building scalable cloud data engineering solutions.

---

## 🚀 Objective

> To build a **real-time analytics platform** using Azure Synapse, demonstrating my ability to architect, develop, and visualize data workflows from ingestion to reporting.

Key goals:
- Leverage both **batch and near real-time processing** via Synapse Pools.
- Demonstrate seamless integration across Azure Synapse, Cosmos DB, and Power BI.
- Transform and model massive datasets to power **business intelligence** dashboards.

---

## 🧠 Key Learnings and Outcomes

- ✅ Designed a **modern data lakehouse architecture** using Azure Synapse Analytics.
- ✅ Ingested NYC Taxi data using **Serverless SQL Pools and Spark Notebooks**.
- ✅ Built **ETL pipelines** and orchestrated jobs via **Synapse Pipelines** and **Triggers**.
- ✅ Enabled **Synapse Link** for Cosmos DB to perform **HTAP (Hybrid Transactional and Analytical Processing)**.
- ✅ Created **dedicated SQL pools** to store transformed data for high-performance querying.
- ✅ Developed **Power BI dashboards** to visualize trip metrics, locations, vendors, and fares.
- ✅ Automated workflows to scale processing for enterprise use cases.

---

## 🧰 Tools & Azure Services

| Azure Service                         | Role in Pipeline |
|--------------------------------------|------------------|
| **Azure Synapse Analytics**          | Unified data integration, transformation, and analytics platform. |
| **Serverless SQL Pool**              | Lightweight, on-demand SQL for raw data exploration and transformation. |
| **Dedicated SQL Pool**               | High-throughput relational data warehouse for reporting workloads. |
| **Apache Spark Pools**               | Distributed computing engine for large-scale data transformation. |
| **Synapse Pipelines**                | Workflow orchestration for ETL and automation. |
| **Azure Data Lake Storage Gen2**     | Data lake storage for raw, cleaned, and curated datasets. |
| **Azure Cosmos DB + Synapse Link**   | Operational analytics from transactional NoSQL data. |
| **Power BI**                         | Dashboarding and data visualization. |

---

## 📦 Architecture Overview

```plaintext
          ┌────────────────────────┐
          │ NYC Taxi Data (Public)│
          └────────────┬───────────┘
                       ▼
       ┌─────────────────────────────┐
       │ Azure Data Lake Gen2        │
       │ - Raw Layer                 │
       └────────────┬────────────────┘
                    ▼
     ┌───────────────────────────────┐
     │ Serverless SQL / Spark Pool   │
     │ - Clean, Transform, Join      │
     └────────────┬──────────────────┘
                  ▼
     ┌───────────────────────────────┐
     │ Dedicated SQL Pool            │
     │ - Curated Reporting Layer     │
     └────────────┬──────────────────┘
                  ▼
     ┌───────────────────────────────┐
     │ Power BI                      │
     │ - Dashboards & KPIs          │
     └───────────────────────────────┘
