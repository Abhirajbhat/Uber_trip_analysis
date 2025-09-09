# 🚖 Uber Trip Analysis (Jan–Feb Dataset)

## 📌 Project Overview
This project analyzes Uber trip data from **January and February** using data preprocessing, exploratory data analysis (EDA), feature engineering, and machine learning modeling.  
The goal is to **understand ride patterns, vehicle activity, and predict trips** using historical data and engineered features.

---

## 📂 Dataset
- **File Used:** `Uber-Jan-Feb-FOIL.csv`  
- Contains daily Uber trip information including:
  - `date` → Date of record  
  - `trips` → Number of trips on that day  
  - `active_vehicles` → Number of active vehicles  

---

## 🛠 Tools & Libraries
- **Python**
- **Libraries**:
  - `numpy`
  - `pandas`
  - `matplotlib`
  - `seaborn`
  - `scikit-learn`

---

## 🔎 Steps Performed
### 1. Data Preprocessing
- Converted `date` column to datetime format.
- Handled missing values and duplicates.
- Created new features like:
  - `day`, `month`, `weekday`
  - `trips_per_vehicle`

### 2. Exploratory Data Analysis (EDA)
- Trips trend over time  
- Active vehicles over time  
- Average trips per vehicle by weekday  
- Correlation heatmap  
- Trip distribution  

### 3. Feature Engineering
- Lag features (`trips_lag1`, `vehicles_lag1`)  
- Rolling averages (7-day trend)  
- Weekend indicator  
- Month names  

### 4. Machine Learning Model
- Model: **Linear Regression**  
- Features used:  
  `active_vehicles, trips_lag1, vehicles_lag1, trips_rolling7, vehicles_rolling7, is_weekend`  
- Target: `trips`  

### 5. Model Evaluation
- **Metrics:**  
  - MAE (Mean Absolute Error)  
  - RMSE (Root Mean Squared Error)  
  - R² Score  

- **Visualizations:**  
  - Actual vs Predicted Trips  
  - Scatter Plot (Predicted vs Actual)  
  - Residual Distribution  
  - Feature Importance  

---

## 📊 Results
- The model was able to predict trips with **good accuracy**.  
- **R² Score** indicates strong correlation between predicted and actual values.  
- `active_vehicles` and lag/rolling features played a crucial role in prediction.  

---

## 🚀 Future Scope
- Apply **time-series forecasting models** like ARIMA, SARIMA, or Prophet.  
- Extend analysis for longer time periods.  
- Add external factors (weather, events) to improve predictions.  

---

## 👤 Author
**Abhiraj Bhat**  
Aspiring Data Scientist

---
