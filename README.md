# Seasonal Agriculture Performance Analysis

**VOIS AICTE Batch 1 (2026–2027) — Major Project**

A data analytics project exploring how agricultural performance varies across seasons — **Kharif, Rabi, and Zaid** — using a farm-level dataset covering environmental conditions, resource usage, crop yield, and economic outcomes.

---

## 📌 Problem Statement

Agricultural activities are influenced by seasonal variations in environmental conditions, farming practices, resource availability, and market conditions. As a result, agricultural performance may differ from one season to another. However, raw agricultural data does not clearly explain how performance changes across seasons or what patterns can be observed under different seasonal conditions.

This project analyzes the given agricultural dataset to investigate seasonal differences in performance by identifying meaningful patterns, trends, relationships, and variations within the available data.

## 🎯 Objective

- Explore and clean a 4,000-record agricultural dataset
- Examine how performance varies across seasons
- Identify seasonal patterns and relationships between environmental conditions and outcomes
- Apply statistical testing to confirm which seasonal differences are significant
- Derive evidence-based insights and recommendations for seasonal agricultural planning

## 📂 Dataset

`seasonal_agriculture_performance_dataset.csv` — 4,000 farm-level records covering:

- **Geography:** 8 states, 10 districts
- **Crops:** 8 crop types
- **Seasons:** Kharif, Rabi, Zaid
- **Irrigation methods:** Drip, Flood, Rainfed, Sprinkler
- **Variables:** rainfall, temperature, humidity, sunlight, soil properties, fertilizer/pesticide use, seed quality, yield, production, cost, revenue, profit, water usage, and disease/pest risk

## 🛠️ Tools & Technologies

- **Python 3** — core language
- **Pandas & NumPy** — data cleaning and feature engineering
- **Matplotlib & Seaborn** — exploratory data visualization
- **SciPy (stats)** — Kruskal-Wallis hypothesis testing
- **Jupyter Notebook** — analysis environment and documentation

## 📁 Repository Structure

```
├── Seasonal_Agriculture_Performance_Analysis.ipynb            # Main analysis notebook
├── seasonal_agriculture_performance_dataset.csv                # Dataset
├── Major Project_Seasonal Agriculture Performance Analysis..pdf # Project brief / problem statement
├── VOIS_Major_Project_PPT_Mallepula_Prashanthi (1).pptx        # Project presentation (PPT)
└── README.md                                                    # Project overview
```

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/seasonal-agriculture-performance-analysis.git
   cd seasonal-agriculture-performance-analysis
   ```
2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scipy jupyter
   ```
3. Launch the notebook:
   ```bash
   jupyter notebook Seasonal_Agriculture_Performance_Analysis.ipynb
   ```

> The notebook reads the CSV from the same folder using a relative path, so keep both files together.

## 🔍 Analysis Workflow

1. **Data Cleaning** — missing value imputation (season + crop-aware medians), duplicate checks, IQR-based outlier capping
2. **Feature Engineering** — profit margin %, cost/revenue per hectare, NPK intensity
3. **Exploratory Data Analysis** — environmental conditions, resource usage, yield, economic performance, and disease/pest risk across seasons
4. **Cross-Analysis** — crop × season and state × season patterns
5. **Correlation Analysis** — relationships between key numeric variables
6. **Statistical Testing** — Kruskal-Wallis H-tests to confirm significance of seasonal differences
7. **Insights & Recommendations** — evidence-based conclusions for seasonal agricultural planning

## 📊 Key Findings

- Environmental conditions (rainfall, temperature, humidity) differ sharply by season and drive most downstream effects
- Yield, profit margin, and water efficiency show statistically significant seasonal variation (confirmed via Kruskal-Wallis testing)
- Crop performance interacts strongly with season — some crops clearly outperform in specific seasons
- Zaid season shows the highest irrigation dependence due to low natural rainfall

## 💡 Recommendations

- Adopt season-specific crop planning based on crop × season performance patterns
- Prioritize efficient irrigation investment for the Zaid season
- Allocate pest-management resources based on season-specific disease/pest risk
- Use profit margin (not just raw profit) to compare efficiency across farms and seasons

## 👤 Author

**Mallepula Prashanthi**
Matrusri Engineering College

## 📄 License

This project was created for academic purposes as part of the VOIS AICTE program.
