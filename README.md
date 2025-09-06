# Bellabeat Case Study – Google Data Analytics Capstone

This repository hosts my **Bellabeat case study** for the Google Data Analytics Professional Certificate.  
The analysis explores Fitbit user activity, sleep, and weight data to generate actionable insights for the **Bellabeat app**.

---

## 🔗 Live Report
- **Interactive HTML (GitHub Pages):** (https://gerardoab111.github.io/Coursera---Bellabeat-Case-Study/)  
- **Source RMarkdown (.Rmd):** `case_study_bellabeat.Rmd`
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

## 📊 Results

### Daily Steps

- **Distribution:** Most users take 0–12,000 steps/day, peaking around 10,000. Few exceed 20,000 steps.  
- **Weekday vs Weekend:** Activity levels are similar; no major difference.  
- **Trend over time:** Steps gradually stabilize around 7,000–8,000/day.  
- **Business Insight:** Segment messaging for active vs. less active users. Encourage sustainable step goals and reward consistency.

### Calories Burned

- Median calories burned: ~2,200–2,300/day.  
- Weekday and weekend patterns are similar.  
- **Insight:** Step count correlates moderately with calories (r ≈ 0.59). Educate users on combining steps with intensity for better results.

### Sleep

- Average sleep: 6.9 h (weekdays) vs 7.3–7.7 h (weekends); efficiency ~91%.  
- Outliers show very short (<5 h) or long sleep (>10 h).  
- **Insight:** Promote consistent sleep routines, alert users to irregular patterns, and emphasize sleep quality over quantity.

### Hourly Activity

- Two peaks in steps: morning (7–9 a.m.) and evening (5–8 p.m.). Low activity during night and early afternoon.  
- Weekend peaks occur later and last longer.  
- **Insight:** Schedule in-app challenges and notifications during peak hours; encourage movement during low-activity periods.

### Weight & BMI

- Avg weight: 72.5 kg; avg BMI: 25.4 (overweight); avg body fat: 19.8%.  
- Distribution is bimodal, likely reflecting mixed-gender Fitbit users.  
- Weight trends: modest losses up to -1.5 kg; gains up to +3.9 kg.  
- **Insight:** Focus on personalized weight management, gamified challenges, and female-targeted campaigns.

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
