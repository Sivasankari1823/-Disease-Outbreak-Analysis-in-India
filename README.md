- 🚨 **Outbreak Detection Scatter Plots**: Normal vs. Outbreak cases with extreme events highlighted  

---

## 🔍 **Exploratory Data Analysis**

### 1️⃣ **Temporal Trends**  

- 🌧️ **Dominant Seasonal Pattern**: Most cases occur during **Monsoon season (July-August)**. Pre-Monsoon (April-May) temperature peaks precede Monsoon rainfall peaks, driving outbreaks.  
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
| Cases vs Deaths         | 0.22       |
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

