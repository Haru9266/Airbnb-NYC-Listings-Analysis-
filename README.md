# Airbnb-NYC-Listings-Analysis-
End-to-end Airbnb NYC Listings Analysis using Python, Pandas, EDA and Power BI Dashboard on 48K+ New York City Airbnb listings.

🏠 Airbnb NYC Listings Analysis
 
![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python) 
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow?logo=powerbi) 
![Pandas](https://img.shields.io/badge/Pandas-Data%20Cleaning-green) 
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
 
---
 
## 📌 Project Overview
 
This project performs a complete **Exploratory Data Analysis (EDA)** on 48,870+ Airbnb listings in New York City (2019 dataset). The goal was to understand pricing patterns, room type distribution, and neighbourhood-level trends across all 5 NYC boroughs — and present findings in an interactive Power BI dashboard.
 
---
 
## 🎯 Objectives
 
- Clean and prepare real-world Airbnb data for analysis
- Identify pricing trends across NYC neighbourhoods and room types
- Discover which areas offer the most listings and highest revenue potential
- Build an interactive Power BI dashboard for business stakeholders
---
 
## 🗂️ Dataset
 
| Feature | Details |
|---|---|
| **Source** | [Inside Airbnb — AB_NYC_2019.csv](http://insideairbnb.com/) |
| **Rows** | 48,870 listings |
| **Columns** | 16 features |
| **Key Fields** | `neighbourhood_group`, `room_type`, `price`, `number_of_reviews`, `availability_365`, `latitude`, `longitude` |
 
---
 
## 🛠️ Tools & Technologies
 
| Tool | Purpose |
|---|---|
| **Python** | Data cleaning, EDA, visualizations |
| **Pandas** | Data manipulation |
| **Matplotlib & Seaborn** | Charts and graphs |
| **Power BI** | Interactive dashboard |
 
---
 
## 🔄 Project Workflow
 
```
Raw Data (AB_NYC_2019.csv)
        ↓
Data Cleaning (Python / Pandas)
  • Filled missing values (name, host_name, reviews_per_month)
  • Removed duplicates
  • Removed listings with price = $0
  • Removed minimum_nights > 365 (unrealistic)
  • Fixed data types (last_review → datetime)
        ↓
Exploratory Data Analysis (Python)
  • Room Type Distribution
  • Price Distribution
  • Neighbourhood Analysis (5 boroughs)
  • Geographic Map (latitude/longitude scatter)
  • Correlation Heatmap
  • Top 10 Most-Listed & Most-Expensive Neighbourhoods
        ↓
Exported cleaned files → Power BI Dashboard
  • airbnb_nyc_cleaned.csv
  • area_summary.csv
  • room_summary.csv
        ↓
Interactive Dashboard (Power BI)
  • KPI Cards, Donut Chart, Bar Chart, Map Visual, Slicers
```
 
---
 
## 📊 Key Findings
 
| # | Insight |
|---|---|
| 🏙️ 1 | **Manhattan** has the highest average listing price (~$197), making it the most premium borough |
| 🏘️ 2 | **Brooklyn** has the most total listings, indicating the highest host activity |
| 🛏️ 3 | **Entire home/apt** is the most expensive room type; **Shared rooms** are the cheapest |
| 📍 4 | **Williamsburg** and **Bedford-Stuyvesant** (Brooklyn) are the top 2 most-listed neighbourhoods |
| ⭐ 5 | **Staten Island** has the fewest listings but relatively decent reviews-per-month |
| 💰 6 | Majority of listings are priced **under $200/night**, with outliers going up to $10,000+ |
| 📉 7 | Price and number of reviews show **very low correlation** — expensive listings don't always get more reviews |
 
---
 
## 📁 File Structure
 
```
Pro-7-Airbnb-NYC-Analysis/
│
├── AB_NYC_2019.csv                    ← Raw dataset
├── airbnb_nyc_cleaned.csv             ← Cleaned dataset (used in Power BI)
├── area_summary.csv                   ← Borough-level aggregated data
├── room_summary.csv                   ← Room type aggregated data
│
├── Airbnb_NYC_EDA.ipynb               ← Main Python notebook (EDA + Cleaning)
│
├── charts/
│   ├── room_type_distribution.png
│   ├── Price_distribution.png
│   ├── neighbourhood_analysis.png
│   ├── roomtype_price.png
│   ├── nyc_map.png
│   ├── top_neighbourhoods.png
│   └── correlation_heatmap.png
│
└── pro-7-power-bi-airbnb.pbix         ← Power BI dashboard file
```
 
---
 
## 📸 Dashboard Preview
 
> Power BI Dashboard — Airbnb NYC Listings Analysis

![Airbnb NYC Dashboard](Screenshot%202026-06-16%20155814.png)
The dashboard includes:
- **KPI Cards** — Avg Price ($152), Total Reviews (1M+), Unique Hosts (37K), Total Listings (49K)
- **Donut Chart** — Listings by Room Type
- **Bar Charts** — Listings & Reviews by Room Type
- **Map Visual** — Latitude/Longitude plot of all listings
- **Slicers** — Filter by `neighbourhood_group` and `room_type`
- **Horizontal Bar Chart** — Top neighbourhoods by total listings
---
 
## ▶️ How to Run
 
1. Clone this repository
```bash
git clone https://github.com/haru9266/Pro-7-Airbnb-NYC-Analysis.git
```
 
2. Install required libraries
```bash
pip install pandas numpy matplotlib seaborn
```
 
3. Open and run the notebook
```bash
jupyter notebook Airbnb_NYC_EDA.ipynb
```
 
4. Open `pro-7-power-bi-airbnb.pbix` in Power BI Desktop to view the dashboard
---
 
## 👩‍💻 About Me
 
**Pooja Kumari** — Fresher Data Analyst | New Delhi, India
 
- 🎓 Data Analytics & AI Certification — Ducat Institute, Noida (2026)
- 🔗 GitHub: [github.com/haru9266](https://github.com/haru9266)
- 🌐 Portfolio: [haru9266.github.io/data-analyst-portfolio](https://haru9266.github.io/data-analyst-portfolio)
- 📧 poojak110059@gmail.com
---
 
*⭐ If you found this project helpful, please give it a star!
