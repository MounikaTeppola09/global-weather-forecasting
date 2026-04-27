# Global Weather Forecasting 

## Overview

The objective of this assessment was to analyze a global weather dataset, build forecasting models, generate advanced insights and demonstrate practical data science skills through end-to-end project execution.

The project includes data cleaning, exploratory data analysis, anomaly detection, machine learning forecasting, ensemble modeling and geographical climate insights.

---

## PM Accelerator Mission

PM Accelerator’s mission is to empower future product, AI and technology leaders through hands-on learning experiences, real-world projects and career acceleration opportunities that help candidates build impactful solutions and grow professionally.

---

## Dataset

**Source:** Kaggle Global Weather Repository Dataset

This dataset contains daily weather information for cities around the world and includes weather, environmental and geographical variables such as:

- Temperature  
- Humidity  
- Wind Speed  
- Atmospheric Pressure  
- Precipitation  
- Air Quality Indicators  
- Latitude / Longitude  
- Country / Location Information

---

# Repository Files

```text
Global_Weather_Forecasting_Assessment.ipynb
README.md
requirements.txt
```

---

## Project Objectives

- Clean and preprocess real-world weather data  
- Explore weather trends and correlations  
- Forecast future temperature trends using machine learning  
- Compare multiple regression models  
- Build an ensemble model for higher accuracy  
- Detect anomalies in weather observations  
- Analyze climate, air quality and global weather patterns  

---

# Project Workflow

## 1. Data Cleaning & Preprocessing

- Handled missing values using median/mode imputation  
- Removed duplicate records  
- Converted `last_updated` into datetime format  
- Treated outliers using IQR filtering  
- Standardized numerical features using `StandardScaler`

---

## 2. Exploratory Data Analysis (EDA)

Generated visualizations for:

- Temperature distribution  
- Precipitation distribution  
- Average temperature trends over time  
- Average precipitation trends over time  
- Correlation heatmap  
- Country-wise temperature comparisons  

---

## 3. Basic Forecasting Model

Built a baseline **Linear Regression** model using time-based features from `last_updated`.

### Evaluation Metrics Used:

- MAE (Mean Absolute Error)  
- RMSE (Root Mean Squared Error)  
- R² Score  

---

## 4. Advanced Forecasting Models

Compared multiple machine learning models:

- Linear Regression  
- Ridge Regression  
- Random Forest Regressor  
- Gradient Boosting Regressor  
- Extra Trees Regressor  
- AdaBoost Regressor  
- XGBoost Regressor  

### Best Standalone Model:

**XGBoost**

- R² = 0.6264

---

## 5. Final Ensemble Model

Built a weighted ensemble using:

- XGBoost (50%)  
- Gradient Boosting (30%)  
- Random Forest (20%)

### Final Results:

| Metric | Score |
|--------|-------|
| MAE | 0.4139 |
| RMSE | 0.5344 |
| R² | **0.6310** |

The ensemble model achieved the best overall forecasting performance.

---

## 6. Advanced EDA & Unique Analyses

### Anomaly Detection

Used **Isolation Forest** to detect unusual weather conditions and outliers.

### Climate Analysis

- Monthly global temperature trends  
- Warmest countries comparison  

### Environmental Impact

- PM2.5 air quality correlation with weather variables  
- Air quality density analysis  

### Feature Importance

Used:

- XGBoost Feature Importance  
- Permutation Importance  

Key predictors included:

- Recent temperature history (`temp_lag1`, `temp_lag3_mean`)  
- Pressure  
- Humidity  

### Spatial Analysis

Visualized global temperature and rainfall patterns using latitude and longitude.

### Geographical Patterns

Compared:

- Warmest countries  
- Rainiest countries  

---

# Technologies Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  
- XGBoost  

