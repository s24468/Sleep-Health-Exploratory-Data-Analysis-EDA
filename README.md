# 🛌 Sleep Health & Lifestyle Data Analysis

An Exploratory Data Analysis (EDA) project investigating the impact of lifestyle habits, stress levels, and cardiovascular metrics on sleep quality and sleep disorders.

---

## 📊 Overview

Sleep quality is deeply interconnected with daily lifestyle choices and overall physical health. This project analyzes a dataset of **374 individuals** across **13 health and demographic attributes** to uncover key patterns and correlations driving sleep health.

---

## 🔑 Key Findings

- **Stress vs. Sleep Quality**: Strong negative correlation ($r \approx -0.90$) — higher stress levels heavily impair sleep quality.
- **Sleep Duration**: Strong positive correlation ($r \approx 0.88$) with sleep quality.
- **Cardiovascular Health**: Higher heart rate ($r \approx -0.66$) negatively affects overall sleep performance.
- **Sleep Disorders**: Distinct patterns observed between BMI categories and the occurrence of disorders such as Sleep Apnea and Insomnia.

---

## 📁 Dataset

The dataset (`sleep_health_and_lifestyle_dataset.csv`) contains 374 rows and 13 columns:

- **Demographics**: `Age`, `Gender`, `Occupation`
- **Sleep Metrics**: `Sleep Duration` (hours/day), `Quality of Sleep` (scale 1–10)
- **Health Indicators**: `BMI Category`, `Blood Pressure`, `Heart Rate`, `Stress Level` (scale 1–10)
- **Activity**: `Physical Activity Level` (mins/day), `Daily Steps`
- **Target Condition**: `Sleep Disorder` (*None*, *Insomnia*, *Sleep Apnea*)

---

## 🛠️ Data Preprocessing & Methodology

1. **Missing Value Handling**: Imputed missing values in `Sleep Disorder` with `'None'`.
2. **Feature Engineering**: Split composite `Blood Pressure` values (e.g., `"120/80"`) into separate numeric columns: `Systolic_BP` and `Diastolic_BP`.
3. **Exploratory Analysis**: Computed Pearson correlation matrix across numerical variables.
4. **Data Visualization**:
   - Correlation Heatmap (Seaborn)
   - Sleep Duration vs. Quality Scatter Plot
   - Stress Level across Occupations (Boxplots)
   - Sleep Disorders by BMI Category (Countplots)

---

## 🧰 Tech Stack

- **Language**: Python 3.x
- **Environment**: Jupyter Notebook
- **Libraries**: `pandas`, `numpy`, `matplotlib`, `seaborn`
