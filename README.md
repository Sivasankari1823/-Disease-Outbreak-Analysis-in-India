# 🌡️ **Disease Case Analysis: Temporal, Geographic, and Environmental Trends**

---

## 📄 **Overview**  
This project performs a comprehensive **Exploratory Data Analysis (EDA)** on historical disease case data across India. The analysis investigates **temporal trends, geographic hotspots, seasonal patterns, and environmental correlations**, providing actionable insights for public health interventions. The study also implements **data preprocessing, log transformation, and outbreak detection** to prepare the dataset for downstream modeling and analysis.


---

## 🗂️ **Dataset Description**  
The dataset includes **8985 records spanning multiple years**, covering:

- 🏛️ **state_ut**: State or Union Territory  
- 🌆 **district**: District-level data  
- 📅 **week_of_outbreak**: Week of reported cases  
- 🦠 **Cases and Deaths**: Daily/weekly counts  
- 🌡️ **Environmental variables**: Temperature, Precipitation, Leaf Area Index (LAI)  

> The dataset is highly **skewed**, with most records showing low case counts and a few extreme outliers.
## Dataset Used

- <a href="https://github.com/Sivasankari1823/-Disease-Outbreak-Analysis-in-India/commit/4eae1df0583ac5f5079755d6704d6ef03d45f8a1"> Dataset</a>
---

## 🎯 **Objectives**  

1. 📈 Analyse temporal trends of disease cases to detect seasonal patterns  
2. 🗺️ Identify geographic hotspots with high disease burden  
3. 🌦️ Study the relationship between environmental factors and disease cases  
4. 🚨 Detect outbreak events using anomaly detection methods  
5. 💡 Generate actionable insights for public health planning  

---

## 🛠️ **Methodology**  

- 🧹 **Data cleaning, missing value handling, and type conversion**  
- 📊 **Log transformation** to normalize skewed Cases distribution  
- 🕒 **Temporal aggregation** by month, season, and year  
- 🌍 **Geographic aggregation and heatmap visualization**  
- 📉 **Correlation and scatter plot analysis** of environmental variables  
- 🚨 **Outbreak detection** using anomaly labeling and visual verification  

---

## 📊 **Visualizations**  

- ⏳ **Time Series Plots**: Total cases per year, seasonal patterns  
- 🔥 **Heatmaps**: Cases by Month and Year, top 20 states/districts  
- 📦 **Box Plots**: Seasonal temperature, precipitation, LAI distributions  
- 🗺️ **Geo Scatter Plots**: District-level case concentration  
- 🚨 **Outbreak Detection Scatter Plots**: Normal vs. Outbreak cases with extreme events highlighted  

---

## 🔍 **Exploratory Data Analysis**

### 1️⃣ **Temporal Trends**  

- 🌧️ **Dominant Seasonal Pattern**: Most cases occur during **Monsoon season (July-August)**. Pre-Monsoon (April-May) temperature peaks precede Monsoon rainfall peaks, driving outbreaks.
  ## 📊 Visualizations

### 1️⃣ Seasonal Trend
]<img width="721" height="470" alt="download" src="https://github.com/user-attachments/assets/feb1e374-eb37-4fd1-bdfe-89fafb58a68a" />

- ⚖️ **Case Distribution Skew**: Daily/record-level cases are heavily right-skewed, requiring **logarithmic transformation** for modeling.  
- 📉 **Inter-Annual Volatility**: Significant yearly fluctuations, peaking around 2015. Sporadic major outbreaks persist post-2015.  
- 🦠 **Top Disease Drivers**: Acute Diarrhoeal Disease, Dengue, Cholera, and Malaria  
- 🔥 **Heatmap Confirmation**: High-intensity clusters in July 2015-2016, coinciding with peak Monsoon rainfall  

---

### 2️⃣ **Geographic Hotspots**  

- 🏆 **Top 5 High-Burden States**: West Bengal, Delhi, Uttar Pradesh, Maharashtra, Karnataka  
- 🌆 **District Concentration**: New Delhi > South 24 Parganas > Bareilly  
- 🗺️ **Geospatial Distribution**: Cases concentrated in northern and eastern regions, confirmed via geo-scatter plots  

---

### 3️⃣ **Environmental Correlation Analysis**  

- 🌡️ **Temperature**: Peaks in April-May, drops during Monsoon  
- 🌧️ **Precipitation**: Peaks sharply in July-August, coinciding with highest case counts  
- 🌿 **Vegetation Health (LAI)**: Peaks in October (Post-Monsoon)  

**Correlation Summary:**  

| Variable Pair           | Correlation |
|-------------------------|------------|
| Cases vs Deaths         |  0.22       |
| Temperature vs Precip   | -0.35      |
| Temperature vs LAI      | -0.33      |
| Precipitation vs Longitude | 0.20    |

> Weak linear correlations suggest **non-linear or lagged relationships**, or masking due to population density/geography.

---

### 4️⃣ **Case Distribution & Outbreak Detection**  

- ⚖️ **Data Skew**: Most days are low-case, confirming rarity of high-case events  
- 🚨 **Outbreak Identification**:  
  - Outbreaks labeled based on extreme deviations from baseline  
  - Peaks in **2009 (>50,000 cases)** and **2019 (>35,000 cases)**  
  - Elevated activity around 2015-2016, multiple events >5,000 cases  
- 🌧️ **Rainfall Lag Analysis**: Weekly rainfall in preceding 1-4 weeks does not strongly predict immediate case spikes  

---

## 💡 **Project Insights**  

- 🌧️ **Seasonal Patterns**: Highest cases during **Monsoon season**  
- 🌡️ **Environmental Correlation**: Temperature & precipitation moderately negative correlation with cases (-0.35)  
- 🏙️ **High-Burden Locations**: New Delhi reports highest cases  
- ⚖️ **Cases vs. Deaths**: Weak positive correlation (0.22)  
- 🗺️ **Geographic Concentration**: West Bengal, Delhi, Uttar Pradesh, Maharashtra, Karnataka  
- 🚨 **Outbreak Detection**: Extreme years include 2009 and 2018  

---

## 🏁 **Conclusion**  

The analysis reveals that disease outbreaks in India exhibit **strong seasonal patterns**, with Monsoon season experiencing the highest burden. Correlation analysis shows **weak to moderate relationships** between environmental factors and disease cases. Geographic hotspots require **targeted interventions**, and findings emphasize **tailored public health strategies**, including **water management, sanitation, and vector control** during high-risk periods.

