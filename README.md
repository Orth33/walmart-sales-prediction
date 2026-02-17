# 🛒 Walmart Sales Prediction

A machine learning project that forecasts weekly Walmart sales using feature engineering and tree-based ensemble models.


## 📌 Project Overview

This project builds a complete sales forecasting pipeline using:

- Data merging & preprocessing
- Feature engineering (time-based features)
- Random Forest Regression
- XGBoost Regression
- Seasonal time-series analysis

The goal is to predict `Weekly_Sales` for each store and department combination.


## 📂 Dataset

The dataset consists of:

- `train.csv` – Historical weekly sales
- `features.csv` – External features (Temperature, Fuel Price, CPI, Unemployment, Holidays)
- `stores.csv` – Store metadata (Type, Size)



## ⚙️ Workflow

### 1️⃣ Data Preparation
- Merge datasets on `Store` and `Date`
- Convert dates to datetime
- Handle missing values

### 2️⃣ Feature Engineering
- Extract Year, Month, Week, Day
- Include economic indicators
- Include holiday flags
- Include store metadata

### 3️⃣ Model Training
- Random Forest Regressor
- XGBoost Regressor

### 4️⃣ Evaluation Metrics
- MAE (Mean Absolute Error)
- R² Score

### 5️⃣ Seasonal Analysis
Time-series decomposition to identify:
- Trend
- Seasonality
- Residual patterns



## 📊 Model Performance

| Model          | MAE | R² Score |
|---------------|------|----------|
| Random Forest | ✔️   | ✔️       |
| XGBoost       | ✔️   | ✔️       |

*(Exact values depend on training run.)*



## 🚀 How to Run

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost statsmodels
```

Then run the notebook:

```bash
jupyter notebook Walmart_Sales_Prediction.ipynb
```



## 📈 Future Improvements

- Add LightGBM model
- Hyperparameter tuning
- Feature importance visualization
- Add lag features for time-series enhancement
- Deploy as a web app



## 🧠 Key Learnings

- Importance of feature engineering in tabular data
- Benefits of gradient boosting over bagging
- Handling time-based data correctly
- Avoiding data leakage in forecasting tasks



## 👩‍💻 Author

Urbana Jaman Orthee  
Engineering Student | Machine Learning Enthusiast

---

⭐ If you found this project helpful, consider giving it a star!
