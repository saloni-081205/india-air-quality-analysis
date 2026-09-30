# 🇮🇳 India Air Quality Intelligence and Analysis System

<div align="center">

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-2.0+-green?style=for-the-badge&logo=pandas)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.3+-orange?style=for-the-badge&logo=scikit-learn)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Complete-success?style=for-the-badge)

**An end-to-end Data Science project analyzing 5 years of air quality data across 26 Indian cities**


</div>

---

## 📋 Overview

Air pollution is a **major health crisis in India** — 14 of the world's 15 most polluted cities are in India. This project provides a comprehensive analysis and prediction system for air quality, helping citizens, researchers, and policymakers understand and act on pollution data.

### 🎯 Objectives

- ✅ Analyze **city-wise pollution patterns** across 26 Indian cities
- ✅ Identify **seasonal and yearly trends** in air quality
- ✅ Determine **which pollutants most affect AQI**
- ✅ Visualize insights through **10+ charts and graphs**
- ✅ Build a **machine learning model** to predict AQI category
- ✅ Create an **interactive prediction system** for real-time AQI forecasting

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 🧹 **Data Preprocessing** | Handles missing values (up to 61%), data type conversion, outlier detection |
| 📊 **Exploratory Data Analysis** | City-wise, seasonal, monthly, and yearly trend analysis |
| 📈 **10+ Visualizations** | Bar charts, line charts, heatmaps, boxplots, scatter plots |
| 🤖 **Logistic Regression Model** | 80.64% accuracy in predicting AQI categories |
| 🎯 **Interactive Predictor** | Real-time AQI category prediction with health advisories |
| 📉 **Statistical Analysis** | Skewness, kurtosis, correlation analysis |
| 🌍 **PAN India Coverage** | North, South, East, West regional analysis |

---

## 📊 Dataset

### Source
- **Dataset:** [Air Quality Data in India (2015-2020)](https://www.kaggle.com/datasets/rohanrao/air-quality-data-in-india)
- **Original Source:** [Central Pollution Control Board (CPCB), India](https://cpcb.nic.in/)

### Statistics

| Attribute | Value |
|-----------|-------|
| **Total Records** | 29,531 rows |
| **Total Features** | 16 columns |
| **Time Span** | 2015 - 2020 (6 years) |
| **Cities Covered** | 26 major Indian cities |
| **Data Points Analyzed** | 26,730 records (after cleaning) |

### Columns

| Column | Description | Unit |
|--------|-------------|------|
| `City` | Name of the Indian city | - |
| `Date` | Date of observation | YYYY-MM-DD |
| `PM2.5` | Fine particulate matter | µg/m³ |
| `PM10` | Coarse particulate matter | µg/m³ |
| `NO` | Nitric oxide | µg/m³ |
| `NO2` | Nitrogen dioxide | µg/m³ |
| `NOx` | Nitrogen oxides | µg/m³ |
| `NH3` | Ammonia | µg/m³ |
| `CO` | Carbon monoxide | mg/m³ |
| `SO2` | Sulfur dioxide | µg/m³ |
| `O3` | Ozone | µg/m³ |
| `Benzene` | Benzene | µg/m³ |
| `Toluene` | Toluene | µg/m³ |
| `Xylene` | Xylene | µg/m³ |
| `AQI` | Air Quality Index | - |
| `AQI_Bucket` | AQI Category | Category |

### Cities Covered
```
Ahmedabad, Aizawl, Amaravati, Amritsar, Bengaluru, Bhopal, Brajrajnagar,
Chandigarh, Chennai, Coimbatore, Delhi, Ernakulam, Gurugram, Guwahati,
Hyderabad, Jaipur, Jorapokhar, Kochi, Kolkata, Lucknow, Mumbai, Patna,
Shillong, Talcher, Thiruvananthapuram, Visakhapatnam
```

---

## 🛠️ Installation

### Prerequisites
- Python 3.8 or higher
- pip package manager
- Jupyter Notebook (for running .ipynb file)

### Step 1: Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/india-air-quality-intelligence.git
cd india-air-quality-intelligence
```

### Step 2: Create Virtual Environment (Recommended)

```bash
# Windows
python -m venv venv
venv\Scripts\activate

# Mac/Linux
python3 -m venv venv
source venv/bin/activate
```

### Step 3: Install Dependencies

```bash
pip install -r requirements.txt
```

### Step 4: Download Dataset

Download `city_day.csv` from [Kaggle](https://www.kaggle.com/datasets/rohanrao/air-quality-data-in-india) and place it in the project root directory.

---

## 📦 Requirements

Create a `requirements.txt` file with these dependencies:

```txt
pandas>=1.5.0
numpy>=1.23.0
matplotlib>=3.6.0
seaborn>=0.12.0
scikit-learn>=1.2.0
jupyter>=1.0.0
notebook>=6.5.0
```

---

## 🚀 Usage

### Running the Jupyter Notebook

```bash
jupyter notebook PDS_OEP_India_Air_Quality_Index.ipynb
```

### Project Workflow

```
┌─────────────────────────────────────────────────────────────┐
│  PHASE 1: DATA UNDERSTANDING & PREPROCESSING                │
│  • Load data → Check missing values → Convert data types    │
│  • Handle missing values → Extract datetime features        │
└─────────────────────────────────────────────────────────────┘
                            ↓
┌─────────────────────────────────────────────────────────────┐
│  PHASE 2: EXPLORATORY DATA ANALYSIS (EDA)                   │
│  • Descriptive statistics → City-wise analysis              │
│  • Seasonal trends → Pollutant correlation                  │
└─────────────────────────────────────────────────────────────┘
                            ↓
┌─────────────────────────────────────────────────────────────┐
│  PHASE 3: VISUALIZATION                                     │
│  • 10+ charts revealing patterns and insights               │
└─────────────────────────────────────────────────────────────┘
                            ↓
┌─────────────────────────────────────────────────────────────┐
│  PHASE 4: MACHINE LEARNING MODEL                            │
│  • Logistic Regression → 80.64% accuracy                    │
│  • Interactive prediction system                            │
└─────────────────────────────────────────────────────────────┘
```

### Interactive Prediction Example

```python
# Run the prediction cell and enter values:
Enter City Name: Jaipur
PM2.5 [default: 54.4]: 50
PM10 [default: 123.1]: 120
NO2 [default: 32.3]: 37
CO [default: 0.8]: 2.4
SO2 [default: 11.1]: 19
O3 [default: 46.5]: 39.7

# Output:
PREDICTED AQI CATEGORY: MODERATE
Confidence: 86.7%

HEALTH ADVISORY:
Unusually sensitive people should reduce outdoor activities.
```

---

## 📈 Results

### Key Findings

| Finding | Insight |
|---------|---------|
| 🏭 **Most Polluted City** | Ahmedabad (Mean AQI: 358) |
| 🌿 **Cleanest City** | Aizawl (Mean AQI: 36) |
| 📅 **Worst Month** | November (AQI: 227) |
| 📅 **Best Month** | July (AQI: 109) |
| ❄️ **Worst Season** | Winter (AQI: 206) |
| 🌧️ **Best Season** | Monsoon (AQI: 112) |
| 🚗 **Strongest Pollutant** | CO (Correlation: 0.677) |
| 📉 **COVID Impact** | 26% AQI drop in 2020 |

### Model Performance

| Metric | Score |
|--------|-------|
| **Overall Accuracy** | **80.64%** |
| Precision (Good/Satisfactory) | 85% |
| Precision (Moderate) | 77% |
| Precision (Poor) | 82% |
| Precision (Severe) | 85% |

### City Rankings

**Top 5 Most Polluted Cities:**
| Rank | City | Mean AQI | Category |
|------|------|----------|----------|
| 1 | Ahmedabad | 358.25 | Severe |
| 2 | Delhi | 250.29 | Very Poor |
| 3 | Lucknow | 218.56 | Poor |
| 4 | Patna | 215.51 | Poor |
| 5 | Gurugram | 212.68 | Poor |

**Top 5 Cleanest Cities:**
| Rank | City | Mean AQI | Category |
|------|------|----------|----------|
| 1 | Aizawl | 36.24 | Good |
| 2 | Shillong | 75.54 | Satisfactory |
| 3 | Coimbatore | 77.92 | Satisfactory |
| 4 | Thiruvananthapuram | 78.15 | Satisfactory |
| 5 | Bengaluru | 91.43 | Satisfactory |

---

## 📊 Visualizations

### Chart 1: Top 10 Most Polluted Cities
> North Indian cities dominate; Ahmedabad and Delhi consistently worst

### Chart 2: Yearly AQI Trend
> COVID-19 lockdown caused dramatic 26% drop in 2020

### Chart 3: Seasonal AQI Variation
> Winter (206 AQI) nearly double the pollution of Monsoon (112 AQI)

### Chart 4: Month-wise Pollution Pattern
> November worst (227 AQI), July best (109 AQI)

### Chart 5: AQI Category Distribution
> Only 5% days are "Good", over 60% days are unhealthy

### Chart 6: Correlation Heatmap
> CO and PM2.5 have strongest correlation with AQI

### Chart 7: PM2.5 vs AQI Scatter Plot
> PM2.5 explains 39% of AQI variation (R² = 0.391)

### Chart 8: AQI Distribution by City (Boxplot)
> Ahmedabad has widest spread; Delhi has highest median

### Chart 9: Pollutant Exceedance
> PM2.5 exceeds safe limits on 33% of days

### Chart 10: Weekday vs Weekend
> Small difference suggests continuous pollution sources

---

## 💡 Key Insights

### 🔴 Critical Findings

1. **Only 1 city (Aizawl) has "Good" average AQI** — rest of India breathes unhealthy air daily
2. **North-South divide:** Northern cities average AQI 200+, Southern cities ~100
3. **CO is the strongest AQI predictor** (0.677 correlation) — vehicle emissions are critical
4. **November is the worst month** — crop burning + Diwali + winter onset
5. **COVID lockdown proves clean air is achievable** — AQI dropped 26% in 2020

### 🎯 Policy Recommendations

| Recommendation | Reasoning |
|----------------|-----------|
| Prioritize vehicle emission control | CO has highest correlation with AQI |
| Winter emergency action (Nov-Feb) | Temperature inversion traps pollutants |
| Focus on PM2.5 reduction | Exceeds safe limits 33% of days |
| Preserve Northeast clean air | Aizawl (36 AQI) is national benchmark |
| Ban stubble burning pre-Diwali | November pollution spike |

---

## 📁 Project Structure

```
india-air-quality-intelligence/
│
├── 📄 README.md                      # This file
├── 📄 requirements.txt               # Python dependencies
├── 📄 LICENSE                        # MIT License
├── 📄 .gitignore                     # Git ignore file
│
├── 📁 data/
│   └── city_day.csv                  # Air quality dataset
│
├── 📁 notebooks/
│   └── PDS_OEP_India_Air_Quality_Index.ipynb   # Main analysis notebook
│
├── 📁 src/
│   ├── preprocessing.py              # Data cleaning functions
│   ├── eda.py                        # Exploratory analysis
│   ├── model.py                      # ML model training
│   └── predict.py                    # Prediction utilities
│
├── 📁 outputs/
│   ├── charts/                       # Generated visualizations
│   │   ├── top_polluted_cities.png
│   │   ├── yearly_trend.png
│   │   ├── seasonal_variation.png
│   │   └── correlation_heatmap.png
│   └── model/
│       └── logistic_model.pkl        # Trained model
│
└── 📁 docs/
    └── PDS_OEP.pdf                   # Project report
```

---

## 🤖 Model Details

### Logistic Regression Model

```python
from sklearn.linear_model import LogisticRegression
from sklearn.preprocessing import StandardScaler
from sklearn.model_selection import train_test_split

# Features
features = ['PM2.5', 'PM10', 'NO2', 'CO', 'SO2', 'O3']

# Split
X_train, X_test, y_train, y_test = train_test_split(
    X, y, test_size=0.2, random_state=42, stratify=y
)

# Scale
scaler = StandardScaler()
X_train_scaled = scaler.fit_transform(X_train)
X_test_scaled = scaler.transform(X_test)

# Train
model = LogisticRegression(max_iter=1000, random_state=42)
model.fit(X_train_scaled, y_train)
```

### Why Logistic Regression?

| Reason | Explanation |
|--------|-------------|
| **Predicts Categories** | AQI is a category (Good/Moderate/Poor), not a number |
| **Probabilistic** | Gives confidence percentages for each category |
| **Fast Training** | Works well with 26,730 samples |
| **Interpretable** | Easy to explain which features matter |

---

## 🔬 Methodology

### Phase 1: Data Preprocessing
- **Missing Values:** Median imputation for numeric, mode for categorical
- **Outlier Detection:** Z-score method (|Z| > 3 = extreme)
- **Feature Engineering:** Extracted Year, Month, Season, DayOfWeek

### Phase 2: Exploratory Data Analysis
- **Descriptive Statistics:** Mean, median, std, quartiles
- **Shape Statistics:** Skewness (3.89), Kurtosis (27.08)
- **Correlation Analysis:** Pearson correlation with AQI

### Phase 3: Visualization
- **10+ Charts:** Bar, line, pie, heatmap, boxplot, scatter
- **Insights:** City patterns, seasonal trends, pollutant impact

### Phase 4: Machine Learning
- **Model:** Logistic Regression (multi-class)
- **Accuracy:** 80.64%
- **Features:** 6 pollutants
- **Output:** AQI category + confidence

---

## 📝 Limitations

| Limitation | Description |
|------------|-------------|
| **80% Accuracy** | 1 in 5 predictions may be wrong |
| **No Weather Data** | Doesn't account for wind, rain, temperature |
| **Historical Data** | Trained on 2016-2020, may not reflect recent changes |
| **City Averages** | Local micro-location may differ |
| **Requires Pollutant Input** | User needs access to pollutant measurements |

---

## 🚧 Future Improvements

- [ ] Add weather data (wind, temperature, humidity)
- [ ] Implement deep learning (LSTM for time-series)
- [ ] Build web app using Streamlit/Flask
- [ ] Add real-time API integration with CPCB
- [ ] Include more recent data (2021-2024)
- [ ] Add forecasting (predict next week's AQI)
- [ ] Interactive dashboard with Plotly/Dash

---

## 👥 Team

**Group No. 8**

| Name | Enrollment No. |
|------|----------------|
| Siddhi Patel | ET23BTCO041 |
| Saloni Rana | ET23BTCO048 |
| Khevana Vasani | ET23BTCO065 |

**Subject:** Python for Data Science (BTCO13602)
**Course:** B.E. III, SEM-VI (Even-2026)

---

## 📚 References

1. [Kaggle Dataset - Air Quality Data in India](https://www.kaggle.com/datasets/rohanrao/air-quality-data-in-india)
2. [Central Pollution Control Board (CPCB)](https://cpcb.nic.in/)
3. [CPCB Real-time AQI Monitoring](https://app.cpcbccr.com/AQI_India/)
4. [World Health Organization - Air Pollution](https://www.who.int/health-topics/air-pollution)

---



