# ⚽ Premier League 2024/25 KPI Analysis

## 📌 Project Overview

This project analyses the 2024/25 Premier League season by transforming raw match-level data into structured team-level performance KPIs, which are then visualised in an interactive Power BI dashboard.

The objective was to build a complete analytical pipeline:

- Ingest raw season data
- Transform match-level data into team-level records
- Aggregate season statistics
- Engineer performance KPIs
- Deliver executive-ready dashboards

This project demonstrates SQL-based data transformation, KPI engineering, and business-focused dashboard design.

---

## 🧱 Data Pipeline Overview

The analytical workflow follows a structured transformation process:

- Raw match data and team reference data were ingested into SQL.
- Match data was enriched by joining team metadata.
- Each match was expanded into two team-level records (home and away).
- Season-level metrics were aggregated per team.
- A league table was constructed and ordered by points.
- Custom KPIs were engineered for analytical use in Power BI.

The final output table (01_data/03_kpi_table.csv) was used as the primary dataset for dashboard development.

---

## 🧮 SQL Transformation

The SQL pipeline performs:

- Table creation and ingestion of raw data
- Match-to-team row transformation
- Points calculation (Win = 3, Draw = 1, Loss = 0)
- Season-level aggregation
- Goal difference calculation
- KPI engineering for dashboard consumption

See:
02_sql/01_premier_league_kpi_pipeline.sql

---

## SQL Transformation Preview

![01_sql_kpi_transformation](04_images/01_sql_kpi_transformation.png)

---

## 📊 Dashboard Overview

### 1️⃣ Executive Overview

![02_overview](04_images/02_executive_overview.png)

Provides a high-level summary of league standings and key performance indicators. Filters selected to demonstrate cross-filtering and slicer functionality, allowing dynamic exploration of team data

---

### 2️⃣ Performance Drivers Analysis

![03_performance_drivers_analysis](04_images/03_performance_drivers_analysis.png)

Explores statistical relationships and drivers of success, including shot conversion, shot quality, and defensive resiliency.

---

### 3️⃣ Key Insights

![04_key_insights](04_images/04_key_insights.png)

Highlights analytical conclusions derived from KPI comparisons and team performance trends.

---

## 🚀 Outcome

This project demonstrates the ability to move from raw datasets to actionable insight using a structured analytical workflow:

Raw Data → SQL Transformation → KPI Engineering → Business Dashboard

It reflects a real-world analytics process, combining technical SQL development with business-focused data visualisation.

---

## 🛠 Tools Used

- SQL (data transformation & aggregation)
- Power BI (data modelling & dashboard visualisation)
- GitHub (version control & documentation)

---

## 🎯 Key Skills Demonstrated

- Data transformation pipeline design
- Relational joins & structured aggregation
- KPI engineering
- Data modelling for BI tools
- Executive-level dashboard presentation
- Analytical storytelling

---

## 📁 Repository Structure

```
premier_league_kpi_analysis/
|
├── 01_data/
│   └── 01_matches_table.csv
│   ├── 02_teams_table.csv
│   └── 03_kpi_table.csv
├── 02_sql/
│   └── 01_premier_league_kpi_pipeline.sql
├── 03_powerbi/
│   └── 01_premier_league_2024_25_kpi_analysis.pbix    
├── 04_images/
│   ├── 01_sql_kpi_transformation.png
│   ├── 02_executive_overview.png
│   ├── 03_performance_drivers_analysis.png
│   └── 04_key_insights.png
└── README.md   
    
    
