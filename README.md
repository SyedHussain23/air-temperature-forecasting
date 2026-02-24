# 🌡️ air-temperature-forecasting

This project builds a **time series forecasting model** to predict future monthly mean surface air temperatures using historical climate data.

It demonstrates a complete **end-to-end forecasting pipeline**, including:

* Data loading and exploration
* Trend analysis and visualization
* Feature engineering for time series modeling
* Model training and evaluation
* Future temperature forecasting

The objective is to forecast **monthly mean air temperature for the next 12 months** using machine learning. The business goal is to develop a predictive model capable of forecasting monthly mean temperature values. 

---

## 📌 Project Overview

* **Problem Type:** Time Series Regression
* **Domain:** Climate Analytics / Environmental Data Science
* **Target Variable:** mean_temp
* **Model Used:** Linear Regression
* **Forecast Horizon:** 12 months

---

## 📊 Dataset

Features:

* **month** → date of observation
* **mean_temp** → monthly average temperature (target)

Dataset link:
[https://d3ilbtxij3aepc.cloudfront.net/projects/AI-Capstone-Projects/PRAICP-1003-AirTempTS.zip](https://d3ilbtxij3aepc.cloudfront.net/projects/AI-Capstone-Projects/PRAICP-1003-AirTempTS.zip)

---

## 🔍 Exploratory Data Analysis

Key findings:

* Clear seasonal temperature pattern
* Gradual warming trend over time
* No missing values
* Rolling average highlights long-term trend

---

## 🔧 Feature Engineering

To convert time series into supervised learning format:

* Extracted **year** and **month_of_year**
* Created sequential **time_step**
* Computed **12-month rolling average**

These features help the model capture seasonal and temporal trends.

---

## 🧠 Model Training

A **Linear Regression model** was trained using:

* year
* month_of_year
* time_step

The dataset was split with the last 12 months reserved for testing.

---

## 📈 Model Evaluation

Metrics used:

* Mean Absolute Error (MAE): **0.588**
* Mean Squared Error (MSE): **0.521**

These results indicate the model can capture temperature patterns with reasonable accuracy.

---

## 🔮 Forecasting

The trained model was used to forecast:

➡️ Monthly mean temperatures for the next 12 months

Future dates were generated and used as input features to produce predictions.

---

## ⚠️ Challenges

* Time series modeling using non-sequential ML model
* Capturing seasonality using engineered features
* Forecast horizon extrapolation
* Limited dataset complexity

---

## 🚀 Future Improvements

* ARIMA / SARIMA models
* LSTM / deep learning forecasting
* Prophet model
* Hyperparameter tuning
* Lag feature engineering
* Cross-validation for time series

---

## 🚀 How to Run

```bash
git clone https://github.com/SyedHussain23/air-temperature-forecasting
cd air-temperature-forecasting
pip install -r requirements.txt
jupyter notebook air-temperature-forecasting.ipynb
```

---

## 👨‍💻 Author

**Syed Hussain Abdul Hakeem**

* GitHub: [https://github.com/SyedHussain23](https://github.com/SyedHussain23)
* LinkedIn: [https://www.linkedin.com/in/syed-hussain-abdul-hakeem](https://www.linkedin.com/in/syed-hussain-abdul-hakeem)

---

## ⭐ Support

If you found this project useful, consider giving it a ⭐.
