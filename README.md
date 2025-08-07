# Healthcare_Insurance_Analysis
The objective of this project is to predict patients’ healthcare costs and to identify factors  contributing to this prediction. It will also be useful to learn the interdependencies of  different factors and comprehend the significance of various tools at various stages of  the healthcare cost prediction process.


This project focuses on analyzing hospitalization data, medical examination records, and patient details to predict healthcare insurance costs. The goal is to identify the key factors that influence hospitalization costs and to build predictive models for better insurance pricing.


##  Problem Statement
Healthcare costs are rising rapidly, and insurance companies struggle to price their plans accurately. By analyzing historical data, we aim to:
- Understand cost drivers (age, conditions, hospitalization factors)
- Build regression models to predict hospitalization costs
- Recommend pricing strategies and health policies

- 

##  Dataset Information
 1. **Hospitalization Details**
- Patient ID
- Hospital stay duration
- Treatments administered
- Total cost incurred

 2. **Medical Examination Data**
- BMI, Blood pressure, Cholesterol, Sugar, etc.
- Smoking, Drinking habits

 3. **Patient Names & Demographics**
- Name, Gender, Age
- Address (state, city)


##  Exploratory Data Analysis (EDA)

- Distribution plots for cost, age, and BMI
- Correlation heatmap to detect multicollinearity
- Comparative boxplots (e.g., smoker vs non-smoker costs)
- Outlier detection & handling


##  Hypothesis Testing
- Do smokers incur higher hospitalization costs?
- Is there a significant cost difference between male and female patients?
- Does age group affect insurance claims?



##  Feature Engineering
- Extracted age from DOB
- Created binary variables for smoker, drinker
- One-hot encoded categorical variables (e.g., city/state)

---

##  Machine Learning Models

| Model | MAE | RMSE | R² |
|-------|-----|------|----|
| Linear Regression | 2423 | 3021 | 0.71 |
| Ridge Regression | 2408 | 3000 | 0.72 |
| Gradient Boosting | 2178 | 2770 | 0.80 |

 Final model: **Gradient Boosting Regressor** performed best.



 ##  Key Insights

- Smoking and high BMI are strong cost indicators
- Age > 60 tends to have 40% higher hospitalization costs
- Early detection (regular checkups) reduces cost by ~25%



##  Tech Stack
- **Python** (Pandas, NumPy, Matplotlib, Seaborn)
- **Scikit-Learn** (Regression, Cross-Validation, Pipelines)
- **Jupyter Notebook**
- **GitHub**


##  Repository Structure
Healthcare_Insurance_Analysis/
│
├── data/
│ ├── hospitalization.csv
│ ├── Medical Examinations.csv
│ └── names.csv
│
├── notebooks/
│ └── Healthcare_Insurance_Analysis_New.ipynb
│
├── README.md



