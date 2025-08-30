# ✈️ Airline Weather Delay EDA

This project explores airline delay data with a focus on **weather-related delays**.  
It was completed as part of the Statistics for Decision Making Exploratory Data Analysis (EDA) coursework.

---
## Structure
```
airline-eda/
├─ notebooks/
│  └─ exploratory_data_analysis.ipynb
├─ data/
│  └─ airline_dataset            
├─ reports/             
├─ README.md
└─ .gitignore
```
## 📝 Objectives

1. **Load and inspect** the dataset (`airline_dataset.csv`).
2. **Calculate central tendency measures** of weather delay percentages:
   - Per-airline mean
   - Per-airline 10% trimmed mean
   - Overall mean and trimmed mean
3. **Visualize distributions** with boxplots of `pct_weather_delay` for all 6 airlines.
4. **Summarize findings** in prose, highlighting differences in performance and the effect of outliers.

---
## 📊 Key Results
- **Overall mean weather-delay share:** 0.68%  
- **Overall trimmed mean (10%):** 0.47%

| Airline   | Mean (%) | Trimmed Mean (%) |
|-----------|----------|------------------|
| Alaska    | 0.51     | 0.23 |
| American  | 1.12     | 0.97 |
| Delta     | 0.68     | 0.45 |
| Jet Blue  | 0.47     | 0.30 |
| Southwest | 0.51     | 0.38 |
| United    | 0.68     | 0.41 |
| **Overall** | **0.68** | **0.47** |

- **American** shows the highest weather-related delays (mean 1.12%) and many outliers.  
- **Jet Blue** and **Alaska** show the lowest delays and the most stable distributions.  
- **United** exhibits extreme outliers (up to ~35%), which inflate its average compared to its trimmed mean.  

---

## 📈 Boxplot Insights

The boxplots of `pct_weather_delay` reveal:
- **Medians** close to 0.5–1% across airlines.
- **American** has a higher median and wider spread.
- **Jet Blue and Alaska** have smaller boxes (more consistent performance).
- **United** has the most extreme outliers, showing occasional severe weather impact.

---
