# 🥤 Coca-Cola (KO) Stock Price Prediction Dashboard

## 📌 Project Overview
The Coca-Cola Company is a multinational beverage giant incorporated in 1892 and headquartered in Atlanta, Georgia. As a prominent component of the Dow Jones Industrial Average, its stock (ticker: **KO**) has been publicly traded since 1919 and serves as a global proxy for market performance. 

This project provides an end-to-end data science solution to analyze historical trends and provide live price forecasts. It features a research-oriented Jupyter Notebook for model selection and a production-ready Streamlit dashboard for real-time predictions.

## 🛠️ Tech Stack
**Language:** Python
**Analysis:** Pandas, NumPy, Matplotlib, Seaborn 
**Machine Learning:** Scikit-Learn (Linear Regression, Random Forest, Decision Trees) 
**Live Data:** Yahoo Finance API (yfinance)
**Deployment:** Streamlit 

## 📊 Key Research Findings
* **Historical Resilience:** Coca-Cola has paid a dividend since 1920 and has increased it for 57 consecutive years as of 2019.
* **Champion Model:** After evaluating multiple algorithms (including Random Forest and Decision Trees), **Linear Regression** was identified as the most accurate model for short-term daily forecasting.
* **Accuracy:** The model achieved a **Mean Absolute Error (MAE) of ~$0.29**, meaning daily predictions are typically within 30 cents of the actual price.
* **Feature Importance:** Today's **Close Price** and **Moving Averages** (20-day and 50-day) were identified as the strongest predictors for the next day's performance.



## 🚀 App Features
* **Live Data Streaming:** Automatically fetches the latest market data using the Yahoo Finance API.
* **Technical Indicators:** Interactive visualization of short-term (20-day) and long-term (50-day) Moving Averages.
* **Tomorrow's Forecast:** Uses the trained champion model to predict the next trading day's closing price.
* **Market Insights:** Displays current volatility and returns based on rolling windows.



## 📂 Project Structure
* `Notebook.ipynb`: Contains the Exploratory Data Analysis (EDA), feature engineering, and model comparison.
* `app.py`: The production-ready Python script for the Streamlit web dashboard.
* `Coca-Cola_stock_history.csv`: Historical dataset used for training and initial research.

## 🚦 How to Run
1. **Install Dependencies:**
   pip install streamlit yfinance pandas scikit-learn matplotlib seaborn
2. **Run the Analysis:** Open Notebook.ipynb in Jupyter to view the research and model comparison.
3. **Launch the App:**
   streamlit run app.py


## Analyst Conclusion
This project successfully transitions from a raw historical dataset to a live-updating predictive tool. By implementing Target Shifting to prevent data leakage and identifying the superior performance of Linear Regression for this specific ticker, the system provides a robust, data-driven approach to monitoring Coca-Cola's stock movements.