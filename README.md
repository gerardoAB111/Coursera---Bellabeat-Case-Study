# Bellabeat Case Study – Google Data Analytics Capstone

This repository hosts my **Bellabeat case study** for the Google Data Analytics Professional Certificate.  
The analysis explores Fitbit user activity, sleep, and weight data to generate actionable insights for the **Bellabeat app**.

---

## 🔗 Live Report
- **Interactive HTML (GitHub Pages):** [View Report](https://gerardoab111.github.io/Coursera---Bellabeat-Case-Study/)  
- **Source RMarkdown (.Rmd):** [View in repo] 
---

## 🎯 Business Task
Bellabeat wants to better understand how consumers use smart devices (e.g., Fitbit) in order to identify usage trends. The objective is to apply these insights to one of Bellabeat’s products and improve its marketing strategy, ultimately supporting the company’s growth in the global wellness technology market.

**Key Deliverables:**

- Analyze smart device usage data (Fitbit dataset) to identify consumer behavior trends.
- Apply insights to one selected Bellabeat product (Leaf, Time, Spring, or the Bellabeat App).
- Generate high-level marketing recommendations to improve customer engagement and retention
---

## 🛠️ Case Study Framework
This project follows the six key phases of the Google DA capstone:

1. **Ask** – Define the business problem and objectives  
2. **Prepare** – Collect and organize the data (Fitbit dataset)  
3. **Process** – Clean, structure, and validate the data  
4. **Analyze** – Identify trends, patterns, and insights  
5. **Share** – Communicate findings via reports and visualizations  
6. **Act** – Recommend actions to support Bellabeat’s strategy  

---

## 📦 Scope and Data
- **Product focus:** Bellabeat App (chosen product for applying insights and recommendations).  
- **Timeframe:** Fitbit dataset, March–May 2016 (sourced from Kaggle).  
- **Sample size:** ~30 participants across multiple tables.  
- **Source:** [Fitbit Fitness Tracker Data (Kaggle, CC0)](https://www.kaggle.com/datasets/arashnic/fitbit)  
---

## 📊 Data Dictionary
**`daily_activity.csv`**  
- `Id` – User ID  
- `ActivityDate` – Date  
- `TotalSteps`, `TotalDistance`, `Calories`  
- `VeryActiveMinutes`, `FairlyActiveMinutes`, `LightlyActiveMinutes`, `SedentaryMinutes`  

**`sleep_day.csv`**  
- `Id` – User ID  
- `SleepDay` – Date  
- `TotalMinutesAsleep`, `TotalTimeInBed`, `TotalSleepRecords`  

**`weight_log.csv`**  
- `Id` – User ID  
- `Date` – Timestamp  
- `WeightKg`, `BMI`, `IsManualReport`, `Fat` (often missing)  

**`hourly_steps.csv`**  
- `Id` – User ID  
- `ActivityHour` – Timestamp (hourly)  
- `StepTotal` – Steps in that hour  

---

## 🧹 Data Cleaning & Preparation
- Standardized column names and date-time types  
- Removed duplicates and anomalies  
- Aligned date keys across tables before joining  
- Engineered new features (sleep efficiency, activity intensity buckets)  
- QA checks: NA handling, row counts, range sanity checks  

---

## 🔑 Key Insights
- Users with more consistent **sleep** show higher **next-day activity**.  
- **Weekday activity** peaks midweek; weekends dip in steps.  
- A minority of users log **weight/sleep consistently**, biasing results.  

---

## 📌 Recommendations
- **Sleep nudges:** bedtime reminders, streak rewards, morning recaps  
- **Activity challenges:** weekday micro-challenges, contextual prompts  
- **Personalization:** send nudges at times aligned with user history  

---

## ⚠️ Limitations
- Small, non-representative sample (~30 Fitbit users, 2016 data)  
- Fitbit ≠ Bellabeat user base  
- Missing/uneven logs (esp. sleep & weight)  
- Insights are **directional**, need validation with Bellabeat’s real user data  

---

## 👤 Contact
**Author:** Gerardo Abarca  
📧 abarcagerardoj777@gmail.com 
💼 https://www.linkedin.com/in/gerardo-abarca-2389b6328/
