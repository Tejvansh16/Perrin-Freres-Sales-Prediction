# 🥂 Perrin Freres Sales Prediction  

Time series forecasting of monthly champagne sales using ARIMA and SARIMAX models.  

---

## 📌 Project Overview  
This project involves building a time series forecasting model to predict the monthly sales of Perrin Freres champagne using historical data from **1964 to 1972**. The goal is to capture trends and seasonality for accurate sales predictions, aiding in inventory management and decision-making.  

### ✅ **Key Objectives:**  
- Perform time series analysis to identify trends and seasonality.  
- Apply statistical tests to ensure stationarity of the data.  
- Build and optimize ARIMA and SARIMAX models.  
- Generate accurate sales forecasts for future planning.  

---

## 🗂 Dataset  
- **Data:** Monthly champagne sales from 1964 to 1972.
- **Link** [https://www.kaggle.com/datasets/anupamshah/perrin-freres-monthly-champagne-sales](https://www.kaggle.com/datasets/anupamshah/perrin-freres-monthly-champagne-sales?select=perrin-freres-monthly-champagne.csv)
- **Columns:**  
  - `Month`: Time in **YYYY-MM** format.  
  - `Sales`: Champagne sales in millions.  
- **Observations:** 105 data points.  

---

## 🛠 Tech Stack  
- **Programming Language:** Python  
- **Libraries:** Pandas, NumPy, Statsmodels, Matplotlib, Seaborn  
- **Models:** ARIMA, SARIMAX  
- **Evaluation Metrics:** AIC, BIC  

---

## 🚀 Approach  

1. **Data Preprocessing:**  
    - Cleaned the dataset by removing missing values.  
    - Converted the time data to datetime format for proper analysis.  

2. **Exploratory Data Analysis (EDA):**  
    - Visualized sales data to identify seasonal trends and spikes.  
    - Applied **Autocorrelation (ACF)** and **Partial Autocorrelation (PACF)** to analyze lag correlations.  

3. **Stationarity Testing:**  
    - Performed the **Augmented Dickey-Fuller (ADF) Test** to check for stationarity.  
    - Applied **first-order differencing** and **seasonal differencing** to make the data stationary.  

4. **Model Building:**  
    - Built an **ARIMA (1,1,1)** model for non-seasonal patterns.  
    - Developed a **SARIMAX (1,1,1)x(1,1,1,12)** model to capture both trend and seasonality.  

5. **Evaluation:**  
    - Evaluated model performance using:  
      - **AIC:** 1911.627  
      - **BIC:** 1919.560  
    - Generated forecasts for future sales using the SARIMAX model.  

---

## 📊 Results and Visualizations  

- Visualized actual vs predicted sales using line plots to observe the accuracy of forecasts.  
- Identified seasonal spikes, particularly during holiday months, using SARIMAX predictions.  

---
