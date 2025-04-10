## 📊 Amazon Stock Forecasting with SARIMAX  

### 🔹 Overview  
This Python script retrieves **Amazon stock price data** from **Yahoo Finance API via RapidAPI**.  
The data is in **JSON format**, which is converted into a structured **Pandas DataFrame** for analysis.  

### 🛠 Data Processing  
- Extracts **Amazon stock price** for the past **5 years** at a **weekly frequency**.  
- Performs **statistical tests** to determine **seasonality and trend presence**.  
- Since seasonality is present, the **SARIMAX model** was selected for forecasting.  

### 🔍 Model Selection  
- The stock data exhibits **homoskedastic behavior**, meaning stationarity enforcement wasn’t necessary.  
- **Hyperparameter tuning** initially caused **memory issues**.  
- To resolve this, any **problematic configurations** triggering warnings were **sent to garbage collection**, improving efficiency.  

### 🚀 Optimization & Improvements  
- Garbage collection significantly **enhanced performance**, making model tuning more effective.  
- Final model provides **future stock price forecasts** based on historical trends.  

### 🔗 Running the Script  
To execute this script, **you must obtain your own API key** from **RapidAPI** to access Yahoo Finance data.  

