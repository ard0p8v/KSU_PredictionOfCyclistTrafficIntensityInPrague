# Prediction of Cyclist Traffic Intensity (Prague)

This project focuses on predicting the **hourly intensity of cyclist traffic**
using open data from the **Golemio API (Prague)**.
The goal is to demonstrate the full data science workflow:
from data collection and preprocessing to feature engineering,
model training, and evaluation.

The project was created as part of a university course focused on machine learning
and time series analysis.

---

## Data Source

- Open data provided by **Golemio API**
- Bicycle counters and their hourly detection records
- Data are aggregated into an **hourly time series** for a selected location

---

## Project Workflow

The notebook follows a clear and reproducible pipeline:

1. **Data acquisition**
   - Downloading bicycle counter metadata
   - Fetching detection data via REST API with pagination

2. **Data preprocessing**
   - Conversion to time series format
   - Handling missing timestamps
   - Imputation of missing values

3. **Feature engineering**
   - Time-based features (hour, day of week, weekend)
   - Lag features
   - Rolling statistics

4. **Modeling**
   - Naive baseline model (lag-based)
   - Linear Regression (baseline ML model)
   - Gradient Boosting Regressor (non-linear model)

5. **Evaluation**
   - Comparison using MAE and RMSE
   - Visual comparison of predicted vs. actual values

---

## Technologies Used

- Python
- pandas, numpy
- scikit-learn
- matplotlib
- Jupyter Notebook

---

## 📈 Results

The models are evaluated and compared using error metrics and visualizations.
The results show that more advanced models (Gradient Boosting)
outperform naive and linear baselines, especially in capturing non-linear patterns
in cyclist traffic behavior.

