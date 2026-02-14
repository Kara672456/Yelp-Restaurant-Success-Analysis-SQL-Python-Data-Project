# Yelp Restaurant Success Analysis

[![Yelp Dataset](https://img.shields.io/badge/Dataset-Yelp%20Academic-brightgreen)](https://www.yelp.com/dataset)
[![Python](https://img.shields.io/badge/Python-3.9%2B-blue)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-2.x-green)](https://pandas.pydata.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow)](LICENSE)

**Data-driven investigation** linking **user engagement (reviews, tips, check-ins)** to **restaurant success (star ratings, review counts)** using Yelp Academic Dataset. Analyzed **31,537 open restaurants** across **47 cities**.[file:2][file:1]

## 🎯 Project Overview

In the competitive restaurant industry, this analysis reveals **how engagement drives success**:

- **Strong correlation**: Reviews ↔ Success Score **r=0.82**[file:2]
- **70% engagement boost**: High-rated (≥3.5★) restaurants get **4.5x more** reviews/tips/check-ins[file:2]
- **Philadelphia leads**: Success Score **42.65** (top city)[file:2]
- **Seasonal peaks**: December reviews **+18%** above average[file:2]
- **Consistency > bursts**: Steady engagement predicts long-term success[file:2]

**Key Insight**: *Volume trumps sentiment*—1,000 reviews > 100 perfect ones.[file:2]

## 📊 Key Findings

| Metric          | High-Rated (≥3.5★) | Low-Rated (<3.5★) | Correlation w/ Success |
|-----------------|--------------------|-------------------|------------------------|
| **Avg Reviews** | **72**            | **42 (+70%)**    | **0.82**[file:2]      |
| **Avg Tips**    | **10**            | **7**            | **0.71**[file:2]      |
| **Avg Check-ins**| **122**          | **89**           | **0.68**[file:2]      |
| **Success Score**| **38.9+**        | **22.3**         | -[file:2]             |

**🏆 Top 5 Cities** (Success Score):
1. Philadelphia, PA: 42.65
2. Tampa, FL: 41.27
3. Indianapolis, IN: 39.02
4. Tucson, AZ: 38.69
5. Nashville, TN: 39.74

   
## 🛠 Tech Stack
🔧 Language: Python 3.9+
📊 Data: Pandas, NumPy, SQLite3
📈 Viz: Matplotlib, Seaborn
🔬 Stats: SciPy, Statsmodels
⚡ Tools: Jupyter Notebook

## 📈 Featured Visuals

1. **Engagement Heatmap**: Reviews-Tips-Checkins correlations (0.7-0.9)[file:1]
2. **Time Trends**: 2017+ high/low-rated (Dec peaks)[file:1] 
3. **Geo Maps**: Folium city success heatmaps[file:1]


📥 Files:
| File                                        | Description       |
| ------------------------------------------- | ----------------- |
| Analysis-notebook.ipynb[file:1]             | Full EDA + Code   |
| Yelp-Restaurant-Analysis-Report.pdf[file:2] | Executive Summary |
| yelp.db                                     | SQLite Database   |

💡 Actionable Recommendations
For Restaurant Owners
Monthly Targets: 5+ new reviews (small), 20+ (large)[file:2]

Multi-Channel: Promote tips + check-ins alongside reviews[file:2]

Holiday Boost: +30% budget Q4 (Oct-Dec peaks)[file:2]

For Investors
Engagement Valuation: Success Score >40 = 3.5x higher performance[file:2]

Geo Priority: PA/FL markets (+3-10% metrics)[file:2]

🔬 Hypotheses Results (All ✅ Confirmed)
| Hypothesis                       | Evidence                             |
| -------------------------------- | ------------------------------------ |
| H1: High engagement → success    | r=0.68-0.82, p<0.001[file:2]         |
| H2: Positive sentiment → ratings | Compliments r=0.38[file:2]           |
| H3: Consistency > bursts         | Time-series stability r=0.67[file:2] |
| H4: Geographic variation         | 3-10% state differences[file:2]      |

## 📚 Methodology Highlights
#### 🔍 Data: 31,537 restaurants (IQR outliers removed)
#### 📏 Success Score: rating × log(reviews+1)
#### 📊 Correlations: Pearson (0.68-0.82)
#### ⏱️ Trends: STL Decomposition (2006-2021)
#### 🗺️ Geo: Folium heatmaps (47 cities)
