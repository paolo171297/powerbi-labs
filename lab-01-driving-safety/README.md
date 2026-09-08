# 🚗 Lab 01: Driving & Road Safety Analysis

## 🎯 Overview & Objectives
This exercise focuses on combining multi-year traffic data from separate text files and folders using **Power Query**, and creating a **Line and Stacked Column Chart** in Power BI Desktop to analyze fatalities vs. miles traveled.

---

## 🔄 ETL & Power Query Steps
- **Data Merging:** Joined `Mileage2018` and `Fatalities2018` on `State` and `Year`.
- **Data Appending:** Combined multi-year datasets into a single query (`DrivingSafely2007-18`).
- **Folder Import:** Dynamically loaded and transformed an entire folder of historical `.txt` files.

---

## 📊 Visualizations & Formatting
- **Combo Chart:** Displays **Miles (Millions)** as columns and **Fatalities** as a line trend.
- **Line Interpolation:** Configured the line formatting to **Linear** (instead of Smooth) for accurate data representation without visual overshoot.
- **Slicer:** Added a State slicer for interactive filtering.

---

## 🖼️ Dashboard Preview

<a href="https://raw.githubusercontent.com/paolo171297/powerbi-labs/main/lab-01-driving-safety/Practice-Activity-10.svg" target="_blank">
  <img src="https://img.shields.io/badge/View%20Full%20SVG-0078D4?style=for-the-badge&logo=powerbi&logoColor=white" alt="View Full SVG">
</a>
<a href="https://raw.githubusercontent.com/paolo171297/powerbi-labs/main/lab-01-driving-safety/Practice%20Activity%2010.pbix" download>
  <img src="https://img.shields.io/badge/Download%20.PBIX-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Download PBIX">
</a>

<br><br>

<img src="./Practice-Activity-10.svg" alt="Practice Activity 10 Dashboard Preview" width="100%">
