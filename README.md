# Future-Stock-Prediction
Use historical stock data to predict the next day's closing price. Dataset: Stock market data from Yahoo Finance (retrieved using the yfinance Python library)
**Stock Price Prediction using Machine Learning (TSLA)**

---

### **Introduction**

This project focuses on predicting the **next day stock closing price** using machine learning. The dataset is collected from Yahoo Finance using the `yfinance` library. It contains historical stock market data of Tesla (TSLA) including Open, High, Low, Close, and Volume. The goal is to analyze trends and predict future stock prices using a regression model.

---

### **Steps Performed**

---

### **1. Data Loading**

The stock market data was downloaded using the `yfinance` API for Tesla (TSLA) from 2020 to 2025 and converted into a Pandas DataFrame for analysis.

---

### **2. Data Exploration (EDA)**

Basic dataset information was analyzed, including:

* First and last rows of data
* Dataset shape and structure
* Column names
* Data types (`info()`)
* Statistical summary (`describe()`)
* Missing values check

---

### **3. Data Visualization**

Several visualizations were created to understand data patterns:

*  Stock Closing Price Trend (time series movement)
*  Trading Volume Trend (market activity)
*  Correlation Heatmap (relationship between features)

These visualizations help in understanding how stock features are related.

---

### **4. Data Cleaning**

* Removed missing values using `dropna()`
* Selected important features:

  * Open
  * High
  * Low
  * Close
  * Volume

---

### **5. Feature Engineering**

A new target variable was created:

* **Target = Next Day Closing Price**

This converts the problem into a supervised learning regression task.

---

### **6. Data Splitting**

The dataset was split into:

* 80% Training Data
* 20% Testing Data

Shuffle was disabled because stock data is time-dependent (time series data).

---

### **7. Model Training**

A **Linear Regression model** was used to predict stock prices.
It learns the relationship between input features and the next day closing price.

---

### **8. Model Evaluation**

The model was evaluated using:

* **Mean Absolute Error (MAE)** → Measures average prediction error
* Comparison between actual vs predicted values

---

### **9. Prediction Visualization**

A final graph was plotted to compare:

*  Actual Stock Prices
*  Predicted Stock Prices

This helps visually analyze model performance.

---
---



