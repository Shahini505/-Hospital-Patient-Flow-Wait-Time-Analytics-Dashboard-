
Hospital-Patient-Flow-Wait-Time-Analytics-Dashboard
🏥 Hospital Patient Flow & Wait Time Analytics Dashboard
Project Overview
This Power BI project provides a comprehensive analysis of hospital operations, focusing on patient flow, wait time efficiency, and patient satisfaction scores. The dashboard allows hospital administration to identify bottlenecks in specific departments (e.g., Neurology, Cardiology), track peak admission periods, and correlate wait times with patient experience ratings.

The goal is to move from reactive management to data-driven decision-making to improve the quality of care and operational efficiency.


📊 Dashboard Visuals
1. Patient Flow & Overview (The Pulse)
A high-level view of total patient volume, admission trends, and wait time categories. Patient Flow Screenshot (Replace with the actual path to your first screenshot)

2. Bottleneck & Root Cause Analysis
Advanced analysis using Decomposition Trees and Scatter Plots to find why delays happen. Bottleneck Analysis Screenshot

🔍 Key Features & Insights
[cite_start]KPI Metrics: Tracking of 9,216 total patients with an average satisfaction score of 5.00/10 and an average wait time of 35.26 minutes[cite: 1].
[cite_start]Root Cause Analysis (AI Visual): utilized the Decomposition Tree to break down Average Wait Time by Department and Age Group, identifying that the Neurology department has the highest average wait time (36.80 min) compared to General Practice[cite: 3].
[cite_start]Correlation Analysis: A Scatter Plot (Wait Time vs. Satisfaction) reveals a clear inverse relationship—departments with lower wait times generally record higher patient satisfaction scores[cite: 2].
[cite_start]Peak Traffic Detection: Monthly trend analysis highlights significant admission spikes in March 2024 and August 2024, enabling better staff rostering for future peaks[cite: 2].
Wait Time Segmentation: Patients are categorized into Low, Medium, and High wait time groups. [cite_start]11.74% of patients fall into the "High" category, representing the primary target for process improvement[cite: 2].
🛠 Tech Stack & Methodology
Tool: Microsoft Power BI Desktop
Data Processing (ETL): * Used Power Query to clean raw hospital records.
Converted Admission Date and Wait Time to appropriate data types for time-intelligence analysis.
Created conditional columns to segment patients into Age Groups (Child, Adult, Senior).
Data Modeling: * Designed a Star Schema data model.
Established One-to-Many relationships between Dimension tables (dim_department, dim_patient) and the Fact table (fact_visits).
DAX Measures:
Avg Wait Time = AVERAGE(fact_visits[Wait Time])
Satisfaction Score = AVERAGE(fact_visits[Satisfaction Score])
Total Patients = COUNTROWS(fact_visits)
🎨 UI/UX Design "The Clinical Theme"
[cite_start]Navigation: Implemented a custom right-rail navigation panel using buttons and bookmarks for seamless page switching ("Patient Flow," "Bottleneck Analysis," "Wait Time Trends")[cite: 2].
Color Palette: precise "Medical Blue" theme (Deep Navy background #0B1E3B with Clinical Blue accents) to reduce eye strain and maintain professional aesthetics.
Glassmorphism: Used semi-transparent visual containers to create depth and separation from the background.
📂 How to Run This Project
Download the manoj powebi.pbix file from this repository.
Open the file in Microsoft Power BI Desktop.
Interact with the slicers (Department, Age Group, Gender) on the right side to filter the data.
👤 Author
Bandaru Shahini Aspiring Data Analyst | Power BI Developer*
