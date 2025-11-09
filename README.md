# 🚲 CitiBike Demand Analysis – MGT 585 Group Project

### 📊 Objective
To find the optimal number of bikes to stock at each station at the beginning of the day to maximize total daily trips.

### 🧹 Data Preparation
- Converted categorical variables into factors: `DemandTime`, `DayOfWeek`, `Month`.
- Imputed missing values using **mean imputation** to preserve dataset integrity.
- Detected and removed outliers using the **IQR method** to ensure accurate model training.

### 📈 Descriptive Analysis
- **Demand peaks** mid-week (Wednesday, Thursday).
- **Seasonal effect:** Highest demand from **May–October**, lowest in winter.
- **Top neighborhoods:** Chelsea, Hell’s Kitchen, Greenwich Village.
- **Temperature correlation:** Warmer days and evenings show higher bike usage.

### 🤖 Predictive Modeling
**Regression Formula:**  
`Demand ~ Month + DayOfWeek + Temperature:DemandTime + StartStationId + EndStationId + StartNeighborhood + StartNeighborhood:DemandTime + StartNeighborhood:StartPerCapitaIncome`

- **R² = 0.66**, indicating strong model performance.
- Key predictors: `DemandTime`, `Month`, `Temperature`, and `StartNeighborhood`.
- Evening temperature interaction shows a significant **negative effect** on demand.

### 🧩 Prescriptive Insights
- Allocate bikes strategically across high-demand neighborhoods.
- Increase stocking levels during warmer months and weekday peaks.

---

👥 **Team Members**  
Priyanka Maruti Erande • Lahari Sameeraja Gadi • Raghu Varun Kancharla • Jay Vipul Bharodia • Vedant Joshi • Dilip Kevin Vayya  

📅 **Course:** MGT 585 – Business Performance Analysis  
🏫 **DePaul University**

---

**Technologies:** R, ggplot2, dplyr, regression modeling, data visualization  
**Output:** Descriptive, predictive, and prescriptive insights for bike demand optimization.
