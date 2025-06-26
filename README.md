# 🪙 Bitcoin Price Prediction using Linear Regression 

This project demonstrates how to predict the closing price of Bitcoin using historical daily data and a simple machine learning model.

---

## 📌 Overview

* **Dataset:** Daily Bitcoin prices from 2013 to present
* **Goal:** Predict the **closing price** using features like opening price, daily high, and daily low
* **Algorithm Used:** Linear Regression
* **Tools:** Python, Pandas, Scikit-learn, Matplotlib, Seaborn

---

## 🔄 Workflow

### 1. Data Loading

* CSV file is read using **pandas**

### 2. Data Cleaning

* Column names standardized
* Date column converted to `datetime` format
* Rounded prices to 2 decimal places
* Checked for missing and duplicate values (none found)

### 3. Model Building

* Features: `24h_open`, `24h_high`, `24h_low`
* Target: `closing_price`
* Model: `LinearRegression()` from Scikit-learn

### 4. Evaluation

* ✅ **Mean Absolute Error (MAE):** \~51.5
* ✅ **Mean Squared Error (MSE):** \~14181
* ✅ **R² Score:** **0.99** (Excellent fit)

### 5. Visualization

* Regression plot between `24h_open` and `closing_price`

---

## 📂 Folder Structure

```
bitcoin-price-prediction/
│
├── Bitcoin Price.csv
├── bitcoin_prediction.ipynb
├── README.md
```

---

## 📊 Result

> The model achieved an R² score of **0.99**, meaning it can very accurately predict the closing price based on the input features.

---

## 🛠 Tech Stack

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn

---

## 🔮 Future Improvements

* Try non-linear models (Random Forest, XGBoost)
* Use time series models (ARIMA, LSTM)
* Build a real-time dashboard with Streamlit or Flask

---



