# Lab 02: Computer Login & Workday Time Analysis

## 🎯 Overview & Objectives
This project analyzes employee login and session data to inspect workstation utilization, session durations, and user activity periods. The dataset was cleaned, transformed, and enriched using **Power Query**, followed by the implementation of custom metrics and interactive visuals in **Power BI Desktop**.

---

## 🛠️ Data Processing & Power Query Steps

* **Data Ingestion:** Loaded the `Computer login` dataset from `PowerBIData.xlsx`.
* **Date & Duration Transformations:**
  * Extracted the date component from `Log in` to create `Date of Login`.
  * Computed login session duration (`Log out` minus `Log in`) and converted the total duration into hours (`Duration in Hours`).
* **Row Indexing:** Added an incremental Index column starting from `1`.
* **Role Classification:** Enriched the model by adding a conditional `Role` column distinguishing **Supervisors** (*Mia Wilson*, *Mila Murphy*) from **Data Analysts**.
* **Time Period Segmentation:** Categorized login timestamps into daily shifts using M logic:
  * **Morning:** 06:00 - 11:59
  * **Afternoon:** 12:00 - 17:59
  * **Evening:** 18:00 - 21:59
  * **Late Evening / Early Morning:** 22:00 - 05:59

---

## 📊 Visualizations & Dashboard Design

* **Stacked Column Chart:** Visualized login activity over time, plotting `Date of Login` against total logged hours (`Duration in Hours`).
* **Role & Shift Breakdown:** Enhanced the visualization by segmenting metrics by `Role` (Supervisor vs. Data Analyst) and time periods (`Morning`, `Afternoon`, `Evening`, `Late Evening/Early Morning`).
* **Interactive Slicers & Filters:** Implemented dynamic filtering to compare work patterns across role types and daily time slots.

