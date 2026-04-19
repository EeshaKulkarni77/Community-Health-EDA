# Community Health EDA Analysis

## Overview

This project focuses on exploratory data analysis (EDA) of community health parameters to understand the factors influencing quality of life.

The analysis combines:
- Statistical techniques
- Data visualization
- Regression modeling

The goal is to extract meaningful insights from structured health data and identify patterns that can inform healthcare decisions.

---

## Dataset

- Records: 347  
- Features: 12  

The dataset includes:

**Demographic Features**
- Age  
- Gender  
- Socioeconomic Status (SES)  

**Health & Activity Metrics**
- Step Frequency  
- Stride Length  
- Joint Angle  
- EMG Activity  

**Healthcare Access**
- Service Type (Rehab, Preventive, Consultation)  
- Visit Frequency  

**Target Variables**
- Patient Satisfaction (1–10)  
- Quality of Life Score (50–100)  

---

## Data Preprocessing

- Checked for missing values and inconsistencies  
- Dropped irrelevant identifiers  
- Encoded categorical variables using label encoding  
- Prepared data for statistical analysis and modeling  

---

## Exploratory Data Analysis

### Distribution Analysis
- KDE plots used to analyze distribution of quality of life across gender  
- Histograms used to understand feature distributions  

Example:
- The KDE plot shows overlapping distributions of quality of life scores across genders, indicating minimal variation (see report visualization).

---

### Comparative Analysis
- Box plots used to compare quality of life scores across categories  
- Gender-based comparison showed similar median and spread in QL scores (see page 7 visualization) :contentReference[oaicite:0]{index=0}  

---

### Statistical Concepts Applied

#### Central Limit Theorem (CLT)
- Demonstrated how sample means approach a normal distribution with increasing sample size  
- Used to validate distribution assumptions (page 9) :contentReference[oaicite:1]{index=1}  

#### Bayes Theorem
- Applied to compute conditional probabilities  
- Example: Probability of a participant having high quality of life given gender (page 9–10) :contentReference[oaicite:2]{index=2}  

---

## Modeling & Analysis

### Regression Analysis

- Built linear regression models to study relationship between age and quality of life  

#### Key Findings:
- Positive correlation between age and quality of life up to age 60  
- Negative correlation observed beyond age 60  

Regression Equation:
QL_Score = 70.91 + 0.11 * Age - 1.71 * Service Type

:contentReference[oaicite:3]{index=3}  

---

## Key Insights

- Most participants have mid to high quality of life (mean ≈ 74)  
- Gender does not significantly impact quality of life distribution  
- Age is a significant factor influencing quality of life  
- Therapeutic interventions improve quality of life across demographics  
- After age 60, quality of life tends to decline  

---

## Technologies Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  

---

## Project Structure

├── Community_Health_EDA.ipynb

├── README.md


---

## How to Run

1. Clone the repository: `git clone https://github.com/EeshaKulkarni77/Community-Health-EDA.git`
2. Open the notebook: `Community_Health_EDA.ipynb`
3. Run all cells  

---

## Key Takeaways

- EDA is critical for understanding real-world datasets  
- Statistical methods complement machine learning insights  
- Data interpretation is as important as model building  
- Simple models can reveal meaningful patterns when used correctly  

---

## Future Improvements

- Expand dataset with more participants  
- Apply advanced predictive models  
- Perform feature importance analysis  
- Build interactive dashboards for visualization  

---

## Disclaimer

This project is intended for analytical and educational purposes and does not represent clinical or medical advice.
