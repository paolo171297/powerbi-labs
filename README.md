# 📊 Power BI Labs (PL-300)

A curated collection of hands-on Power BI projects, DAX patterns, Power Query ETL workflows, and study notes compiled while working toward the **Microsoft Certified: Power BI Data Analyst Associate (PL-300)** certification.

---

## 🎯 Repository Overview

This repository acts as a practical laboratory and portfolio for data analysis, data modeling, and business intelligence visualization using Microsoft Power BI.

The contents are structured around the core functional areas covered in the **PL-300** exam:
- **Prepare the Data** (Power Query, M, Data Cleaning & Transformation)
- **Model the Data** (Star Schemas, Relationships, DAX, Time Intelligence)
- **Visualize and Analyze the Data** (Report Design, Formatting, Interactivity, UX)
- **Deploy and Maintain Assets** (Row-Level Security, Workspace Management)

---

## 🛠️ Tech Stack & Skills

- **Core Tool:** Microsoft Power BI Desktop
- **Data Modeling:** Star Schema Design, Snowflake Schema, Granularity Management
- **Analytics & Logic:** DAX (Data Analysis Expressions), Filter Context Manipulation, Time Intelligence
- **Data Transformation:** Power Query / M Language
- **Version Control & Docs:** Git, Markdown

---

## 📂 Laboratory Index

| # | Lab Title | Key Concepts & Focus Areas | Preview |
|---|-----------|----------------------------|---------|
| **01** | [Driving & Road Safety Analysis](./lab-01-driving-safety/) | Combo Charts, Formatting Options (Linear vs. Smooth), Time Intelligence | [View Lab](./lab-01-driving-safety/) |
| **02** | *Coming Soon* | *Upcoming topic / Data Modeling* | - |

*(Note: Click on each lab title to explore the full documentation, high-resolution screenshots, DAX measures, and dataset details.)*

---

## 💡 How to Use This Repository

1. **Browse via Browser:** Navigate to any individual lab directory to read the project breakdown, review the business requirements, and examine the DAX measures used.
2. **Interact with Models:** Download the `.pbix` files directly to open them in **Power BI Desktop**, inspect the data model (Relationships view), and test report interactions.

---

## 📌 Featured DAX Patterns

Here are a few re-usable DAX snippets developed throughout these labs:

### Year-over-Year (YoY) Growth Calculation
```dax
Fatalities YoY % = 
VAR CurrentPeriod = [Total Fatalities]
VAR PreviousPeriod = CALCULATE([Total Fatalities], SAMEPERIODLASTYEAR('Calendar'[Date]))
RETURN
DIVIDE(CurrentPeriod - PreviousPeriod, PreviousPeriod, 0)
