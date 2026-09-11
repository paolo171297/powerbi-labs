# Lab 02: Computer Login & Workday Time Analysis

## 🎯 Overview & Objectives
Analyzes employee login patterns, session durations, and shift distributions using **Power Query** for ETL and **Power BI Desktop** for interactive visualizations.

---

## 🛠️ Data Processing & Power Query Steps

* **Data Ingestion:** Imported `Computer login` dataset from `PowerBIData.xlsx`.
* **Date & Duration Calculations:** Extracted `Date of Login` and calculated `Duration in Hours` from `Log in` and `Log out` timestamps.
* **Row Indexing:** Added an incremental index starting from `1`.
* **Role Classification:** Applied conditional logic to assign roles (**Supervisor** for *Mia Wilson* & *Mila Murphy*, **Data Analyst** for others).
* **Time Period Segmentation:** Categorized logins into daily shifts via M logic: **Morning** (06:00-12:00), **Afternoon** (12:00-18:00), **Evening** (18:00-22:00), and **Late Evening / Early Morning** (22:00-06:00).

---

## 📊 Visualizations & Formatting

* **Stacked Column Chart:** Plotted `Date of Login` vs. `Duration in Hours` to track daily activity trends.
* **Role & Shift Breakdown:** Segmented session metrics by `Role` and time periods (**Morning**, **Afternoon**, **Evening**, **Late Evening**).
* **Interactive Slicers:** Enabled dynamic filtering by user role and shift time slots for cross-sectional analysis.
 ---
## 🖼️ Dashboard Preview & Download

<a href="https://raw.githubusercontent.com/paolo171297/powerbi-labs/main/lab-02-computer-login/Practice-Activity-2.svg" target="_blank">
  <img src="https://img.shields.io/badge/View%20Full%20SVG-0078D4?style=for-the-badge&logo=powerbi&logoColor=white" alt="View Full SVG">
</a>
<a href="https://github.com/paolo171297/powerbi-labs/raw/main/lab-02-computer-login/Practice%20Activity%202.pbix" download>
  <img src="https://img.shields.io/badge/Download%20.PBIX-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Download PBIX">
</a>
