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

```
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
```

---

## 📁 Project Structure

```
IPL-Data-Engineering-Project/
├── data/
│   ├── raw/                   # Original IPL datasets
│   └── processed/             # Transformed datasets
├── notebooks/
│   ├── bronze_layer.ipynb     # Raw data ingestion
│   ├── silver_layer.ipynb     # Data cleaning & transformation
│   └── gold_layer.ipynb       # Business-level aggregations
├── scripts/
│   ├── data_ingestion.py
│   └── data_transformation.py
├── visuals/                   # Plots and charts
├── requirements.txt
├── architecture_diagram.png
└── README.md
```

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

Follow these steps to set up and run the project:

### 📥 1. Clone the Repository

```bash
git clone https://github.com/yourusername/IPL-Data-Engineering-Project.git
cd IPL-Data-Engineering-Project
```

### 📦 2. Install Dependencies

Make sure you have Python 3.8+ installed. Then, install the required Python libraries:

```bash
pip install -r requirements.txt
```

### 🧠 3. Prepare the Dataset

Download the IPL dataset from [Kaggle - IPL Dataset](https://www.kaggle.com/datasets/manasgarg/ipl).

Place the following files inside the `data/raw/` folder:
- `matches.csv`
- `deliveries.csv`

### 💻 4. Run the Project on Databricks

1. **Launch your Databricks workspace**.
2. **Create a cluster** (recommended: Spark 3.x runtime with Python 3.x).
3. **Upload Notebooks**:
   - Navigate to the `/notebooks` directory of this project.
   - Import the notebooks into your Databricks workspace.
4. **Configure File Paths**:
   - Update any DBFS or local file paths in the notebooks to match your environment.
5. **Execute the Pipeline in Sequence**:
   - ✅ `bronze_layer.ipynb` – Raw data ingestion into the Bronze layer.
   - ✅ `silver_layer.ipynb` – Cleaning and transforming data in the Silver layer.
   - ✅ `gold_layer.ipynb` – Aggregation and insights generation in the Gold layer.

---

## 💡 Future Enhancements

- Integrate Power BI / Tableau for dashboarding
- Schedule ETL using Apache Airflow or Databricks Jobs
- Add unit tests for transformations
- Real-time ingestion with Kafka

---

## 🤝 Contributing

Contributions are welcome! Feel free to fork the repo and submit pull requests for improvements or bug fixes.

---
## 🙋‍♂️ Connect with Me

- 🔗 [LinkedIn](https://www.linkedin.com/in/your-profile/)
- 📧 your.email@example.com
