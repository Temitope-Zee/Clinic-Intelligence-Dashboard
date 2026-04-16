 Clinic Operations & Revenue Intelligence Dashboard

## 📌 Project Overview
This project demonstrates an end-to-end data engineering and analytics workflow. I transformed a raw, messy dataset of 1,000 clinic appointments into a structured, high-impact dashboard. The project highlights skills in **Python-based ETL (Extract, Transform, Load)**, **Data Cleaning**, and **Business Intelligence with Power BI**.

## 🛠️ Technical Stack
* **Data Processing:** Python (Pandas, NumPy)
* **Development Environment:** Jupyter Notebook
* **Business Intelligence:** Power BI (DAX)
* **Version Control:** Git & GitHub

## 🔄 The Data Pipeline

### 1. Data Cleaning (Python)
The raw dataset contained several "messy" elements that required programmatic intervention:
* **Gender Standardization:** Consolidated varied inputs (e.g., '0', 'F', 'female', 'M', '1') into uniform 'Male' and 'Female' categories.
* **Financial Formatting:** Used Regex to strip currency symbols (£, €, $, Rs) and converted billing amounts into numeric floats for calculation.
* **Date Normalization:** Handled "mixed" date formats to ensure accurate time-based analysis.
* **Handling Nulls:** Implemented mean imputation for missing billing amounts and categorical placeholders for missing demographic data.

### 2. Feature Engineering
To provide deeper insights, I derived new columns:
* **Wait Time (Days):** Calculated the lead time between booking and the actual appointment.
* **Age Grouping:** Categorized patients (e.g., Minor, Young Adult, Senior) to identify demographic revenue trends.
* **Temporal Features:** Extracted 'Day of Week' and 'Month' to analyze clinic peak loads.

### 3. Visualization (Power BI)
I built an interactive dashboard focused on three key operational pillars:
* **Financial Health:** Total Revenue and Average Billing metrics.
* **Operational Efficiency:** Identifying bottlenecks by analyzing average wait times per department.
* **Patient Trends:** Distribution of appointments by gender and follow-up requirements.

## 📈 Key Insights
* **Efficiency Gap:** Certain departments show significantly higher wait times, suggesting a need for staff reallocation.
* **Follow-up Rate:** Approximately 51% of appointments require a follow-up, which serves as a major driver for recurring clinic volume.
* **Peak Volume:** Identified specific days of the week where patient inflow peaks, providing actionable data for administrative scheduling.

## 📂 Repository Structure
* `Clinic_Analysis.ipynb`: The Jupyter Notebook containing all Python ETL logic.
* `final_clinic_data_for_bi.csv`: The cleaned, enriched dataset exported for Power BI.
* `Clinic_Dashboard.pbix`: The Power BI dashboard file.
* `README.md`: Project documentation.
