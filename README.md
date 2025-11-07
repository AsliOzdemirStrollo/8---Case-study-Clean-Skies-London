# 🌤️ Clean Skies London  

## Data Science Case Study — WBS Coding School  

This project explores **London’s air pollution** through time series forecasting — combining **ARIMA**, **SARIMA**, and **Prophet** models to understand and predict nitrogen dioxide (NO₂) concentration trends.  
The main goal was to perform a rigorous analysis and publish the results as a **Medium article**, translating data findings into actionable insights for a cleaner, healthier city.  

📖 **Read the published article →**  
👉 [London’s Air Pollution: What the Data Says About the Past and the Future](https://medium.com/@aslistrollo/londons-air-pollution-what-the-data-says-about-the-past-and-the-future-3f0d74f0aa57)

---

## 🎯 Objective  
To analyze historical air-quality data from London and **forecast NO₂ levels** using multiple time series approaches.  
The project aimed to compare classical statistical methods with modern forecasting techniques and communicate the results through an accessible, data-driven article.  

> 🧠 *From “The Big Smoke” to a data-driven vision of clean air.*

---

## 📂 Repository Contents  
- 📓 **1_Data_Preparation.ipynb** — cleaning and exploring London air-quality data (NO₂, O₃, PM10, PM2.5).  
- 📓 **2_ARIMA_SARIMA_Modeling.ipynb** — statistical modeling and evaluation of ARIMA/SARIMA forecasts.  
- 📓 **3_Prophet_Forecasting.ipynb** — future NO₂ predictions using Prophet, with trend and seasonality analysis.  
- 📂 **Images/** — project visuals and forecast plots featured in the article.  
  - **NO2_trend_plot.png** — long-term decline in NO₂ levels.  
  - **SARIMA_forecast.png** — SARIMA model prediction comparison.  
  - **Prophet_future_forecast.png** — Prophet-based future pollution forecast.  

---

## 🧑‍💻 Approach  

### 1️⃣ Data Exploration & Cleaning  
- Loaded London air-quality dataset containing NO₂, O₃, PM10, and PM2.5.  
- Focused on **NO₂ (nitrogen dioxide)** as it’s the most indicative pollutant of traffic emissions and urban air quality.  
- Resampled data for consistency, handled missing timestamps, and visualized temporal trends.  

### 2️⃣ Statistical Modeling  
- Implemented **ARIMA** and **SARIMA** models to capture trend and seasonality.  
- Evaluated model performance using **MAE**, **RMSE**, and **MAPE** metrics.  
- Visualized how well statistical models fit historical patterns and short-term predictions.  

### 3️⃣ Prophet Forecasting  
- Applied **Facebook Prophet** to extend forecasts into the future.  
- Decomposed data into **trend**, **seasonality**, and **holiday effects**.  
- Generated forward-looking NO₂ predictions with uncertainty intervals.  

---

## 🎧 Results  

### Model Performance Comparison

| Model | MAE | RMSE | MAPE |
|:--|--:|--:|--:|
| **ARIMA** | 5.8777 | 7.1343 | 12.75% |
| **SARIMA** | **3.2601** | **3.9847** | **7.44%** |
| **Prophet (Tuned Model)** | 3.9790 | 4.7084 | 9.30% |

**Interpretation:**  
- **SARIMA** performed best overall, capturing both seasonality and trend with lowest errors.  
- **Prophet** achieved competitive results with strong interpretability and flexibility for long-term forecasting.  
- **ARIMA** served as a baseline, performing worse due to lack of explicit seasonal handling.  

---

## 🌍 Insights & Findings  

### 🔹 Historical patterns  
- NO₂ levels have **declined significantly since 2016**, showing the impact of environmental policies.  
- Clear **seasonality**: higher in winter (heating, traffic) and lower in summer.  

<img src="Images/Screenshot%202025-11-07%20at%2009.48.37.png" alt="Monthly Average NO₂ Levels in London" width="700"/>

*Monthly average NO₂ concentrations in London — showing clear winter peaks and a long-term downward trend.*

---

### 🔹 Seasonal pattern  
<img src="Images/Screenshot%202025-11-07%20at%2015.59.25.png" alt="Seasonal Pattern of NO₂ Concentration in London" width="700"/>

*Seasonal decomposition of NO₂ levels — highlighting recurring yearly cycles and the effects of colder months.*

---

### 🔹 Model results  
- **SARIMA** best captured short-term fluctuations and seasonality.  
- **Prophet** provided flexible long-term forecasts and intuitive trend–seasonality decomposition.  

---

### 🔹 Forecasts  
- Predictions indicate a **continued slow decrease** in NO₂ concentration, assuming current trends persist.  
- However, seasonal peaks remain — clean-air progress depends on sustained emission control and public policy.  

<img src="Images/Screenshot%202025-11-07%20at%2013.08.42.png" alt="NO₂ Forecast Predictions using Prophet and SARIMA" width="700"/>

*Forecast of NO₂ concentrations in London — projecting gradual decline with persistent seasonal variations.*

---

## 🧾 Conclusions (from the Medium article)  

> 📉 **London’s air is getting cleaner — but the work isn’t done.**  
>  
> Data shows a steady improvement in air quality over the last decade, thanks to initiatives like the **Ultra Low Emission Zone (ULEZ)** and the growth of **electric mobility**.  
> Still, pollution patterns highlight that **seasonal and local peaks** persist, particularly during colder months.  
>  
> The analysis emphasizes that forecasting air quality isn’t just about prediction — it’s about **empowering proactive, evidence-based decisions** for public health and sustainability.  
>  
> Ultimately, the project demonstrates how **data science can translate environmental data into actionable insights** that improve everyday life.

---

## 🛠 Tools Used  
1. **Python** — pandas, numpy, statsmodels, prophet  
2. **Matplotlib / Seaborn** — visualization  
3. **scikit-learn** — evaluation metrics (MAE, RMSE, MAPE)  
4. **JupyterLab** — exploration and experimentation  

---

## 📊 Data Source  
This analysis is based on open data provided by the **London Datastore**:  
🔗 [London Average Air Quality Levels Dataset](https://data.london.gov.uk/dataset/london-average-air-quality-levels-ep8rw/)  
The dataset includes historical measurements of major pollutants (NO₂, O₃, PM10, PM2.5) across London.

---

## 🎓 Key Learnings  
1. Combining **classical statistical models** with **modern forecasting tools** yields deeper insight into temporal behavior.  
2. Air pollution follows **strong seasonal patterns**, requiring season-aware models for realistic predictions.  
3. Turning raw data into a **story with societal impact** (via Medium publication) is the core of applied data science.  
4. Visual storytelling enhances accessibility — bridging technical analysis with real-world meaning.  

---

## 💡 Final Summary  
✅ Modeled and forecasted NO₂ air pollution trends in London.  
✅ Compared ARIMA, SARIMA, and Prophet models for interpretability and accuracy.  
✅ Published a complete data narrative connecting **numbers → insights → policy relevance.**

> *Clean data, clear skies — using data science to help London breathe easier.* 🌱  
