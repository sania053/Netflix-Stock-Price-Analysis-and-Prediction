# 📈 Netflix Stock Price Analysis

A time series analysis project focused on modeling and forecasting the 'Close' stock price of Netflix using statistical techniques such as ARIMA. Built as part of the SC475 - Time Series Analysis course at DAIICT under Prof. Mukesh Tiwari.

---

## 📊 Project Overview

Netflix, one of the most influential streaming platforms, has a volatile stock price that makes it an excellent subject for time series analysis. This project involved:
- Understanding the stock data behavior
- Removing anomalies and stabilizing variance
- Applying transformations and statistical modeling
- Selecting an optimal ARIMA model for forecasting

---

## 🛠 Tools & Technologies

- **Python**
- **pandas**, **numpy**, **matplotlib**, **seaborn**
- **statsmodels**, **scikit-learn**
- **Jupyter Notebook**

---

## 🧪 Methodology

### ✅ Data Preprocessing
- Loaded the stock dataset and performed sanity checks
- Removed missing and duplicate values

### 📉 Exploratory Data Analysis
- Distribution analysis showed **right skewness** and **high kurtosis**
- Box plots revealed several **outliers** on the upper side

### 🔍 Outlier Handling
- Used **Interquartile Range (IQR)** method to remove extreme outliers
- Retained only points within `[Q1−1.5×IQR, Q3+1.5×IQR]`

### 🔁 Stationarity Check & Transformation
- Applied **log transformation** to stabilize variance
- Applied **first-order differencing** to remove trend
- Confirmed stationarity via ACF/PACF plots and visual inspection

### 📈 Model Selection
- Evaluated multiple ARIMA(p, d, q) combinations
- Selected **ARIMA(1,1,1)** based on lowest **AIC**
- Residuals resembled white noise (ideal for forecasting)

---

## 📌 Key Takeaways

- Log-differencing effectively removed trend and variance instability
- ARIMA(1,1,1) provided the best fit based on statistical metrics
- ACF/PACF plots were crucial in selecting the right model parameters
- Project demonstrates the use of core time series techniques on real-world financial data


