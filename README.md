# Hospice Patient Referral Performance Dashboard

## Project Overview

This project demonstrates the development of an interactive Power BI dashboard designed to monitor hospice patient referral performance. The dashboard provides healthcare managers and stakeholders with a clear overview of referral trends, patient demographics, referral sources, service demand, and key performance indicators to support informed decision-making.

The project was developed as part of my Power BI Admistractive skills in data preparation, Power Query, DAX, data modelling, and dashboard design. 


# Business Problem

Hospices receive patient referrals from multiple sources, including General Practitioners (GPs), hospitals, community nursing teams, care homes, and patients' families. Without a centralised, real-time reporting solution, it is difficult for managers and clinical teams to:

- Monitor referral volumes
- Understand referral patterns
- Identify delays in referrals
- Analyse patient demographics
- Allocate resources effectively

Limited visibility into referral performance can impact waiting times, operational planning, and ultimately the quality of patient care. 

---

# Objectives

The objective of this project was to build an interactive Power BI dashboard that enables users to:

- Monitor hospice referral performance
- Analyse referral trends over time
- Identify major referral sources
- Understand patient demographics
- Measure referral timeliness
- Support operational and strategic decision-making

The project closely reflects the responsibilities outlined in the Power BI Administrator role by demonstrating end-to-end dashboard development, from data preparation to reporting. 

---

# Dashboard Preview

<img width="1373" height="781" alt="Screenshot 2026-07-23 144119" src="https://github.com/user-attachments/assets/269cbd23-55a0-4533-b823-375fbae62cb8" />

Suggested screenshots:


---

# Dataset

Due to the confidential nature of healthcare data, a synthetic dataset containing **2,809 hospice referrals** was created.

The dataset covers a **two-year period (April 2023 – March 2025)** and was carefully designed to reflect realistic hospice referral patterns using published NHS England, Hospice UK, and NIHR research.

For example:

- National research suggests approximately **40%** of hospice patients are referred within 30 days of death.
- The synthetic dataset closely reflects this with **39%** of referrals occurring within the same timeframe.

Although the data is fictional, the statistical patterns closely resemble real-world hospice referral behaviour. 

---

# Data Preparation

### Data Source

A synthetic healthcare dataset was created because patient-level hospice referral data is not publicly available due to confidentiality requirements.

### Data Cleaning

The dataset was cleaned in Power Query by:

- Removing duplicate records
- Checking for missing values
- Correcting data types
- Standardising category names
- Validating logical consistency

### Power Query

Power Query was used to transform and prepare the dataset before loading it into the Power BI data model.

### Data Model

A dedicated Date table was created to support time intelligence calculations, and relationships were established between the tables to create an efficient star schema.

### DAX Measures

Several DAX measures were created, including:

- Total Referrals
- Average Referral Days
- Median Referral Days
- Referrals Within 30 Days
- Percentage Referred Within 30 Days

To provide a balanced performance view, both the Average and Median Referral Days were included. The median reduces the impact of extreme referral durations while the average highlights the effect of unusually long referral journeys. 

---

# Dashboard Features

## KPI Cards

The dashboard displays four key performance indicators:

- Total Referrals: **2,809**
- Average Referral Days: **64**
- Median Referral Days: **40**
- Referrals Within 30 Days: **39%**

Displaying both the average and median demonstrates that referral durations are positively skewed by a small number of long referral cases.

---

## Referral Trend

I used a line chart shows referral volumes over time.

Key observations include:

- Stable referral activity throughout the year
- Seasonal increases during winter
- Lower referral volumes during summer

These insights support workforce and operational planning.

---

## Referral Source

The dashboard identifies the main referral pathways.

The largest referral sources are:

- Hospitals
- General Practitioners (GPs)
- Community Nursing Teams

This enables managers to strengthen relationships with their most important referral partners.

---

## Diagnosis Group

Cancer accounts for the majority of referrals, reflecting national hospice referral patterns.

The dashboard also highlights referrals for non-cancer conditions, supporting broader palliative care planning.

---

## Local Area

Taunton and Yeovil generate the highest referral volumes, while smaller towns such as Minehead and Chard demonstrate lower but consistent demand.

This information supports community service planning and resource allocation.

---

## Service Type

Hospice at Home represents the largest service area (38%), followed by:

- Day Services
- Inpatient Care

Understanding service demand helps with workforce planning and capacity management.

---

## Age Band

Patients aged **75–84 years** account for the largest proportion of referrals, which aligns with expected end-of-life care demographics.

---

## Outcome

The most common referral outcome is **Ongoing Care**, followed by patients who died at home while receiving hospice support.

Monitoring outcomes helps identify trends and opportunities to improve referral pathways. 

---

# Key Insights

The dashboard revealed several important insights:

- Referral demand varies throughout the year, with slightly higher activity during winter.
- Hospitals and General Practitioners account for the majority of referrals.
- Cancer remains the largest diagnosis group, although non-cancer referrals remain significant.
- Some diagnosis groups experience later referrals than others.
- Referral demand differs across local areas, with Taunton and Yeovil generating the highest referral volumes. 

---

# Recommendations

Based on the findings, the following recommendations were identified:

- Monitor referral performance monthly.
- Work closely with referral partners experiencing delayed referrals.
- Increase awareness campaigns in rural communities.
- Use dashboard insights to support workforce planning.
- Analyse referral trends by diagnosis and local area to improve service delivery. 

---

# Future Improvements

With access to real hospice operational data, future enhancements would include:

- Connecting directly to SQL Server
- Automating scheduled data refreshes
- Implementing Row-Level Security (RLS)
- Publishing reports to the Power BI Service
- Developing separate Executive and Operational dashboards
- Integrating staffing and bed capacity data to analyse service pressure against referral demand 

---

# Tools Used

- Power BI Desktop
- Power Query
- DAX
- Microsoft Excel
- Data Modelling
- Data Visualisation

---

# Repository Contents

```
Hospice-Patient-Referral-Dashboard/

│── README.md
│── Hospice Referral Dashboard.pbix
│── Dataset/
│     └── Synthetic Hospice Referral Dataset.xlsx
│── Images/
│     ├── Dashboard Overview.png
│     ├── KPI Cards.png
│     ├── Referral Trend.png

```

---

## Author

**Kate Ehimwenma Igbinidu**

Data Analyst | Power BI Developer | SQL | Excel | Python

Passionate about transforming data into actionable insights through interactive dashboards and business intelligence solutions.
