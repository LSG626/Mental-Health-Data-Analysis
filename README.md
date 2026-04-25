# Mental Health Risk Analysis Project (End-to-End Data Analytics)

---

## Project Overview

This project presents a complete **end-to-end data analytics solution** focused on analyzing mental health patterns using survey data. It demonstrates the full lifecycle of a data project:

* Data Extraction
* Data Cleaning & Transformation (ETL)
* Data Storage (Database)
* Data Analysis (SQL)
* Data Visualization (Dashboard)

The objective is to identify **mental health risk levels**, understand **behavioral drivers**, and generate **actionable insights**.

---

## Objectives

* Clean and standardize raw survey data
* Build an ETL pipeline using Python
* Store structured data in a relational database
* Perform SQL-based analysis
* Design an interactive dashboard
* Communicate insights effectively

---

## Tools & Technologies

* Python (Pandas)
* MySQL
* Power BI
* Jupyter Notebook

---

## Dataset Description

The dataset contains mental health survey responses with the following fields:

* Timestamp
* Gender
* Country
* Occupation
* self_employed
* family_history
* treatment
* Days_Indoors
* Growing_Stress
* Changes_Habits
* Mental_Health_History
* Mood_Swings
* Coping_Struggles
* Work_Interest
* Social_Weakness
* mental_health_interview
* care_options

### Engineered Features

* **Risk_Score** → Calculated using behavioral indicators
* **Risk_Category** → Classified as High, Medium, or Low

---

## ETL Pipeline

### Extract

* Loaded raw dataset from CSV using Python

### Transform

* Cleaned missing values
* Standardized categorical values (Yes/No formatting)
* Removed inconsistencies and whitespace
* Converted timestamps to datetime format

### Feature Engineering

* Created **Risk_Score** based on:

  * Growing Stress
  * Coping Struggles
  * Mood Swings
  * Changes in Habits

* Created **Risk_Category**:

  * High Risk
  * Medium Risk
  * Low Risk

### Load

* Stored cleaned data into MySQL table:

  * `cleaned_mental_health`

---

## Database Design

### Table: `cleaned_mental_health`

Contains:

* All original fields
* Engineered features

---

## SQL Analysis

### 1. Risk Category Distribution

Analyzed how individuals are distributed across risk levels.

---

### 2. Risk vs Treatment

Compared risk scores with treatment status.

---

### 3. Country-Level Analysis

Identified countries with higher average risk.

---

### 4. Occupation Risk Analysis

Determined high-risk professions.

---

### 5. Behavioral Factors Analysis

Examined behavioral patterns among high-risk individuals.

---

### 6. Demographic Breakdown

Analyzed risk levels by gender.

---

## Data Modeling (Derived Tables)

Created structured tables for dashboard use:

* `risk_category_distribution`
* `risk_vs_treatment`
* `country_risk_analysis`
* `occupation_risk_analysis`
* `behavioral_high_risk`
* `demographic_risk`

These tables improve performance and simplify visualization.

---

## Dashboard (Power BI)

### Title:

**Mental Health Risk Analysis Dashboard**

---

### KPI Section

* Average Risk Score
* Total Respondents
* High Risk Percentage

---

### Visualizations

* Bar Chart → Risk by Occupation
* Pie Chart → Risk Distribution
* Bar Chart → Risk by Country
* Stacked Chart → Behavioral Factors vs Risk
* Gauge → Average Risk Score vs Target

---

### Filters

* Gender
* Country
* Occupation

---

## Key Insights

* High-risk individuals are strongly linked to stress and coping struggles
* Certain occupations show higher mental health risk
* Risk levels vary across countries
* A gap exists between high-risk individuals and those receiving treatment

---

## Recommendations

* Improve access to mental health treatment
* Promote early detection using behavioral indicators
* Implement workplace mental health programs
* Increase awareness and support systems

---

## CV Statement

> Developed an end-to-end data analytics project involving ETL pipeline creation, SQL analysis, and interactive dashboard design to analyze mental health risk patterns and generate actionable insights.

---

##  What Makes This Project Strong

* Real-world dataset
* End-to-end pipeline
* Feature engineering
* SQL + Dashboard integration
* Business-focused insights

---

## Future Improvements

* Add predictive modeling (Machine Learning)
* Automate ETL pipeline
* Deploy dashboard to cloud

---


