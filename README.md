# ⏱️ AEP Energy Consumption Analysis and Forecasting  

## 📌 Project Overview  
This project explores the **historical energy consumption patterns** of the American Electric Power (AEP) dataset, identifies **seasonal trends**, and builds a **forecasting model** to predict future usage.  

It combines **exploratory data analysis (EDA)** with **time series forecasting** to uncover consumption behavior and support energy demand planning.  

---

## 📊 Dataset  
- **Source:** AEP (American Electric Power) hourly energy usage dataset  
- **Frequency:** Hourly  
- **Period Covered:** ~2004–2018  
- **Columns:**  
  - `datetime` — timestamp of the observation  
  - `AEP_MW` — energy usage in megawatts (MW)  

---

## 🎯 Objectives  
1. Perform exploratory analysis to uncover daily, weekly, and seasonal patterns.  
2. Compare weekday vs. weekend consumption behavior.  
3. Build a forecasting model for short-term energy usage.  
4. Visualize patterns and model outputs for interpretability.  

---

## 🔍 Exploratory Data Analysis (EDA)  

### 1. Overall Energy Usage Trend  
<img src="images/time_series.png" alt="AEP Energy Use" width="600"/>  

**Insights:**  
- Clear yearly seasonality.  
- Winter months show higher usage (heating demand).  
- Peaks and troughs align with seasonal weather changes.  

---

### 2. Monthly Average Usage with Trendline  
<img src="images/monthly_seasonality.png" alt="Monthly Average" width="600"/>  

**Observations:**  
- Highest usage: **Jan–Feb** and **Jul–Aug** (heating + cooling).  
- Lowest usage: **Apr–May** and **Oct**.  

---

### 3. Weekday vs Weekend Hourly Behavior  
<img src="images/weekday_weekend.png" alt="Weekday Weekend Heatmap" width="600"/>  

**Findings:**  
- **Morning peak**: 6–8 AM on weekdays.  
- **Mid-afternoon dip**: during working hours.  
- **Weekends**: later peaks, slightly higher overnight usage.  
- **Fridays**: mixed weekday–weekend pattern.  

---

## 📈 Forecasting  

### Prophet Forecast vs. Actual Test Data  
<img src="images/forecast_vs_actual.png" alt="Prophet Forecast" width="600"/>  

**Model:** Prophet  
- Designed to capture **trend + seasonality**  
- Robust to irregularities and missing data  

**Results:**  
- Forecast closely follows seasonal cycles.  
- Short-term predictions align well with historical behavior.  

---

## 🛠 Technologies Used  
- **Python Libraries:** pandas, numpy, matplotlib, seaborn, scikit-learn, prophet, plotly  
- **Visualization:** Matplotlib, Seaborn, Plotly  
- **Forecasting:** Prophet  

---
