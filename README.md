# pyspark-etl-medallion-architecture
# 🏏 IPL Data Engineering Project

An end-to-end data engineering project analyzing **Indian Premier League (IPL)** data using **Apache Spark (PySpark)** and **Databricks**, following the **Medallion Architecture** (Bronze, Silver, Gold layers).

---

## 🚀 Project Overview

This project demonstrates how to build a scalable data pipeline using PySpark on Databricks. The IPL dataset is ingested, cleaned, transformed, and analyzed to extract meaningful insights.

---

## 🧰 Technologies Used

- 🔹 **Apache Spark (PySpark)** – Distributed data processing
- 🔹 **Databricks** – Cloud-based collaborative platform
- 🔹 **Medallion Architecture** – Bronze, Silver, and Gold layers
- 🔹 **Delta Lake** – Data versioning and ACID transactions
- 🔹 **Pandas, Seaborn, Matplotlib** – Visualization libraries
- 🔹 **Amazon S3 / DBFS** – Data storage (local or cloud)

---

## 🏗️ Architecture
             ┌────────────┐
             │  Raw Data  │
             └────┬───────┘
                  │
           [ Bronze Layer ]
    Ingest raw CSVs into Delta Lake

                  │
           [ Silver Layer ]
  Data cleaning, filtering, transformation

                  │
           [ Gold Layer ]
Aggregations, business metrics & insights


---

## 🔍 Key Insights

- 🏅 **Top Batsmen per Season**
- 🎯 **Most Economical Bowlers in Powerplay**
- 🎲 **Impact of Toss on Match Outcomes**
- 📈 **Team Win Percentages Across Seasons**
- 👑 **Player vs Player Matchups**

---

## 📊 Visualizations

- 📌 Runs scored per team and season
- 📌 Wickets taken by top bowlers
- 📌 Batsmen strike rates and averages
- 📌 Toss vs win correlation charts
- 📌 Team vs team performance graphs

Visuals are generated using `matplotlib` and `seaborn`, and stored under the `visuals/` folder.

---

## ⚙️ Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/IPL-Data-Engineering-Project.git
cd IPL-Data-Engineering-Project

```bash
pip install -r requirements.txt



