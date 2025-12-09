# 🚅 SNCF Punctuality & Performance Dashboard

## 📌 Project Overview
This Business Intelligence project analyzes train punctuality and service reliability for **SNCF Voyageurs**. Using **Power BI**, I transformed raw operational data into an interactive dashboard to help stakeholders identify underperforming lines, track delay trends, and quantify the impact on passengers.

## ❓ Business Problem
SNCF Voyageurs needs a centralized and interactive tool to track operational performance, identify underperforming train lines, and understand the real-world impact of delays on passengers. The goal is to move from static reports to a dynamic dashboard that empowers managers to make faster, data-driven decisions.

## 🛠️ Tech Stack
*   **Tool:** Microsoft Power BI
*   **Data Transformation:** Power Query (M Language) for cleaning and modeling.
*   **Analysis:** DAX (Data Analysis Expressions) for complex calculations.
*   **Data Source:** Open Data SNCF.

## 📊 Key Features & Insights

The dashboard is structured into four main pages, each tailored to a specific analytical need:

### 1. Executive Overview (Aperçu)
*   **KPIs:** Global Punctuality Rate, Average Delay (minutes), Passenger-to-Delay Ratio, Percentage of Delayed Trains.
*   **Visuals:** Time-series analysis of monthly punctuality against a target of 90%, and a bar chart identifying the top 5 least punctual lines.

### 2. Line Performance Analysis (Ligne)
*   **Functionality:** Allows users to filter for a specific train line to view its individual performance metrics and compare monthly trends against other lines.
*   **Visuals:** A detailed matrix showing the month-by-month punctuality percentage for every line, enabling easy identification of seasonality and consistent underperformers.

### 3. Delay Deep Dive (Retard)
*   **KPIs:** Total Number of Delays, Worst Performing Month, Breakdown of delays by service (RER vs. Transilien).
*   **Visuals:** A dual-axis line chart showing the trend of delays over time for different services, helping to pinpoint which service is driving the overall delay numbers.

### 4. Passenger Impact Analysis (Passagers)
*   **KPIs:** Estimated Number of Passengers Affected, a custom **Passenger Impact Score**, and a "Overcrowding Risk" score.
*   **Visuals:** A scatter plot that cross-references the percentage of delayed trains with the number of passengers, quickly identifying high-impact events.

## 💡 Data Modeling & DAX Highlights
*   **Data Transformation:** Used **Power Query** to clean the source data, handle data types, and merge different tables.
*   **Custom KPIs:** Wrote **DAX measures** to calculate non-trivial metrics, such as the `Passenger Impact Score` (a weighted average of delay time and passenger numbers) and month-over-month performance changes.

## 📂 How to View
PDF Report: View the static full report in 2024 from the doc/.
Power BI File: Download the .pbix file from the src/ folder to view the interactivity (requires Power BI Desktop).
Microsoft Fabric Link: https://app.fabric.microsoft.com/groups/me/reports/19a5671b-511b-4ae3-b8bc-95dc6262a716?ctid=e5d15069-41a2-48be-a3f3-d7f52db16425&pbi_source=linkShare&bookmarkGuid=f1994d6a-7ca4-4ca3-a578-31f3f9a1aab3

---
Author: LE Minh Quan
