# 📊 India Census 2011 Data Analysis

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/Jupyter-F37726?style=for-the-badge&logo=jupyter&logoColor=white" />
  <img src="https://img.shields.io/badge/Data%20Analysis-FF6B6B?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Statistics-4285F4?style=for-the-badge" />
</p>

---

## 📋 Overview

**India Census 2011 Data Analysis** is a comprehensive exploratory data analysis project analyzing demographic data from India's 2011 Census. Includes data cleaning, statistical analysis, population density comparisons across states and districts, with rich visualizations using Pandas, Matplotlib, and Seaborn.

**Perfect for:** Learning data cleaning, demographic analysis, and population statistics.

---

## 🎯 Project Goals

- 📍 Analyze India's demographic distribution
- 👥 Explore population trends by state and district
- 🏙️ Compare urban vs rural population
- 📈 Examine population density patterns
- 🔍 Identify demographic insights
- 💡 Create actionable visualizations

---

## 📁 Dataset Overview

**Source:** India Census 2011 - Official Government Data

### Key Columns:

| Column | Description |
|--------|-------------|
| `State` | State name |
| `District` | District name |
| `Population` | Total population |
| `Male` | Male population |
| `Female` | Female population |
| `Literacy Rate` | % literacy |
| `Sex Ratio` | Females per 1000 males |
| `Population Density` | Persons per km² |
| `Area` | Geographic area in km² |
| `Urban` | Urban population |
| `Rural` | Rural population |

---

## 🛠️ Tech Stack

| Component | Technology |
|-----------|-----------|
| **Data Processing** | Pandas, NumPy |
| **Visualization** | Matplotlib, Seaborn |
| **Statistics** | SciPy, Statsmodels |
| **Environment** | Jupyter Notebook |
| **Language** | Python 3.8+ |

---

## 📋 Requirements

```bash
pip install pandas numpy matplotlib seaborn jupyter scipy
```

---

## 🚀 Quick Start

### 1. **Clone Repository**
```bash
git clone https://github.com/ShubhamK-0904/IND-Census-2011--analysis.git
cd IND-Census-2011--analysis
```

### 2. **Install Dependencies**
```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### 3. **Run Analysis**
```bash
jupyter notebook IND-Census-2011-Analysis.ipynb
```

---

## 📊 Analysis Sections

### **1. Data Loading & Inspection**
- Load census CSV data
- Display dataset structure
- Check data types and missing values
- Initial statistics

### **2. Data Cleaning**
- Handle missing values
- Remove duplicates
- Data type conversion
- Outlier detection

### **3. Descriptive Statistics**
- Mean, median, mode
- Standard deviation
- Quantile analysis
- Distribution overview

### **4. Population Analysis**
- Total population by state
- Top 10 most populous states
- State-wise population trends
- Population growth rates

### **5. Demographic Breakdown**
- Male vs Female distribution
- Sex ratio analysis
- Gender imbalance regions
- Demographic trends

### **6. Urbanization Analysis**
- Urban vs Rural split
- Urbanization rate by state
- City-wise population
- Migration trends

### **7. Literacy Analysis**
- Literacy rate by state
- Male vs Female literacy
- Literacy disparities
- Education insights

### **8. Population Density**
- Density distribution
- High-density regions
- District-wise density
- Geographic patterns

### **9. Comparative Analysis**
- State rankings
- District comparisons
- Regional variations
- North-South-East-West analysis

---

## 📈 Key Findings (Sample)

> Run notebook for complete analysis

✅ India's 2011 population: 1.21 billion  
✅ Uttar Pradesh: Most populous state  
✅ Sex ratio: 943 females per 1000 males  
✅ Literacy rate: 74.04% (59.3% rural, 84.1% urban)  
✅ Urban population: 31% of total  
✅ Highest population density: Delhi (11,000+ per km²)  
✅ Population growth rate: 1.97% per year  
✅ Gender gap widest in northern states  

---

## 📊 Visualizations Included

- **Bar Charts:** State populations, literacy rates
- **Pie Charts:** Urban-rural split, gender distribution
- **Histograms:** Population density, literacy distribution
- **Scatter Plots:** Density vs literacy, area vs population
- **Heatmaps:** State-wise metrics, correlation matrix
- **Line Graphs:** Trends across states/districts
- **Box Plots:** Distribution by region

---

## 💻 Code Examples

### **1. Load & Inspect Data**
```python
import pandas as pd

df = pd.read_csv('census_2011.csv')
print(df.head())
print(df.info())
print(df.describe())
```

### **2. Top States by Population**
```python
top_states = df.groupby('State')['Population'].sum().sort_values(ascending=False).head(10)
print(top_states)
```

### **3. Sex Ratio Analysis**
```python
df['Sex_Ratio'] = (df['Female'] / df['Male']) * 1000
avg_ratio = df['Sex_Ratio'].mean()
print(f"Average Sex Ratio: {avg_ratio:.2f}")
```

### **4. Visualization**
```python
import matplotlib.pyplot as plt

plt.figure(figsize=(14, 6))
top_10_states.plot(kind='bar', color='steelblue')
plt.title('Top 10 Most Populous States (2011 Census)')
plt.xlabel('State')
plt.ylabel('Population')
plt.xticks(rotation=45)
plt.tight_layout()
plt.show()
```

---

## 🎓 Learning Outcomes

Master these concepts:
- ✅ Data loading and exploration
- ✅ Data cleaning and preprocessing
- ✅ Descriptive statistics
- ✅ Exploratory data analysis (EDA)
- ✅ Statistical comparison techniques
- ✅ Data visualization best practices
- ✅ Demographic data interpretation
- ✅ Report generation

---

## 📊 Project Stats

| Metric | Value |
|--------|-------|
| **States Analyzed** | 28 |
| **Union Territories** | 8 |
| **Districts** | 640+ |
| **Total Population** | 1.21 Billion |
| **Data Points** | 10,000+ |

---

## 🔄 Analysis Workflow

```
Census Data (CSV)
    ↓
Load & Inspect
    ↓
Data Cleaning
    ↓
Exploratory Analysis
    ↓
Statistical Analysis
    ↓
Visualization
    ↓
Insights & Recommendations
```

---

## 🚀 Future Enhancements

- [ ] Comparison with 2001 Census
- [ ] 2021 Census data analysis
- [ ] Predictive population modeling
- [ ] Interactive Tableau dashboard
- [ ] Migration pattern analysis
- [ ] Economic correlation analysis
- [ ] Heatmaps with geographic visualization
- [ ] Report generation (PDF/Excel)

---

## 📚 Data Sources

- [Census of India Official Website](https://censusindia.gov.in/)
- [Government of India Data Portal](https://data.gov.in/)

---

## 🤝 Contributing

Contributions welcome! Please:
1. Fork repository
2. Create feature branch
3. Add improvements
4. Submit pull request

---

## 📝 License

MIT License - see LICENSE file

---

## 👨‍💻 Author

**Shubham Kadam**
- GitHub: [@ShubhamK-0904](https://github.com/ShubhamK-0904)
- LinkedIn: [Shubham Kadam](https://www.linkedin.com/in/shubham-kadam-b8856031a/)
- Email: shubham85kadam@gmail.com

---

<p align="center">
  <strong>⭐ If you found this helpful, give it a star! ⭐</strong>
</p>

<p align="center">
  Made with ❤️ by Shubham Kadam | Last Updated: May 2026
</p>
