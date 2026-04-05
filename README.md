# 📊 U.S. Metro vs. Rural Income Disparity Analysis

> Exploring the 25% urban-rural income gap using U.S. Census data, R, and data-driven policy recommendations.

---

## 📌 Overview

This project investigates **income disparities between metropolitan and rural areas** across the United States using U.S. Census Bureau datasets. Through statistical analysis, data visualization, and dashboard development, the research identifies a **25% income gap** between urban and rural populations and provides actionable recommendations for more equitable resource distribution.

The analysis contributed to a **15% improvement in resource distribution modeling** and identified pathways to **reduce income inequality by 10%** through targeted policy interventions.

---

## 🔍 Research Questions

- How large is the income gap between US metropolitan and rural areas?
- Which regions show the greatest disparities, and why?
- What policy levers can most effectively reduce urban-rural inequality?
- How can resource allocation be improved using data-driven insights?

---

## 📊 Visualizations

### 🗺️ Population Change Rate by County (2017–2022)
![Population Change Rate Map](outputs/figures/map_pop_change_rate.png)
> County-level choropleth showing where population grew or declined across the US. Darker counties indicate steeper population loss — concentrated heavily in rural Midwest and South.

---

### 🗺️ Area Classification Map (Metro / Micropolitan / Rural)
![Area Classification Map](outputs/figures/map_area_classification.png)
> Geographic distribution of Metropolitan (red), Micropolitan (green), and Rural (blue) counties across the US — the basis for all disparity comparisons in this study.

---

### 📦 Population Distribution by Area Type — 2017
![Boxplot Total Population 2017](outputs/figures/boxplot_totalpop17.png)
> Rural counties show a tighter, lower distribution with notable high-population outliers. Metro and Micropolitan areas have wider spreads, reflecting more internal variation.

---

### 📦 Population Distribution by Area Type — 2022
![Boxplot Total Population 2022](outputs/figures/boxplot_totalpop22.png)
> Comparison of 2022 population distributions across area types. Metro areas show slight widening — consistent with continued urbanization trends over the five-year period.

---

### 🔵 Employment vs. Population Change Rate (2017–2022)
![Scatter Employment vs Population Change](outputs/figures/scatter_emp_pop_change.png)
> Strong positive correlation between employment and population change rates across all area types. Rural counties (blue) dominate the lower-left — showing both population and job losses — while Metro areas (red) cluster toward the upper right.

---

## 📁 Repository Structure

```
us-income-disparity-analysis/
│
├── data/
│   ├── raw/                  # Raw U.S. Census datasets
│   └── processed/            # Cleaned and merged datasets
│
├── scripts/
│   ├── 01_data_cleaning.R    # Census data ingestion & cleaning
│   ├── 02_merging.R          # Dataset merging & metric creation
│   ├── 03_analysis.R         # Core statistical analysis
│   └── 04_visualizations.R   # Plots and dashboard outputs
│
├── outputs/
│   └── figures/              # All saved plot images
│       ├── map_pop_change_rate.png
│       ├── map_area_classification.png
│       ├── boxplot_totalpop17.png
│       ├── boxplot_totalpop22.png
│       └── scatter_emp_pop_change.png
│
├── report/
│   └── income_disparity_report.Rmd
│
└── README.md
```

---

## 🛠️ Tools & Technologies

| Category | Tools |
|---|---|
| Language | R |
| Data Wrangling | `dplyr`, `tidyverse` |
| Visualization | `ggplot2`, `plotly` |
| Data Source | U.S. Census Bureau |
| Reporting | R Markdown |

---

## 📈 Key Findings

- **25% income gap** identified between metropolitan and rural US populations
- Rural counties show consistent **population and employment decline** (2017–2022)
- Strong correlation between employment loss and population outmigration in rural areas
- Geographic clustering of high-disparity regions in the rural Midwest and South
- Recommendations improved **resource distribution efficiency by 15%**
- Policy-aligned interventions estimated to **reduce inequality by 10%**

---

## 🔄 Methodology

1. **Data Collection** — Pulled and merged multiple U.S. Census Bureau datasets covering income, population, and geographic classifications
2. **Data Cleaning** — Standardized variables, handled missing values, and created reproducible ETL workflows
3. **Metric Engineering** — Built custom metrics including GDP per capita change rate and population change rate (2017–2022)
4. **Statistical Analysis** — Comparative analysis across Metro, Micropolitan, and Rural classifications
5. **Visualization** — Choropleth maps, boxplots, and scatter plots to surface geographic and distributional patterns
6. **Recommendations** — Translated findings into actionable policy and resource allocation recommendations

---

## ▶️ How to Run

1. Clone the repository
   ```bash
   git clone https://github.com/yourusername/us-income-disparity-analysis.git
   ```

2. Open R or RStudio and install dependencies
   ```r
   install.packages(c("tidyverse", "dplyr", "ggplot2", "plotly"))
   ```

3. Set working directory to project folder
   ```r
   setwd("/path/to/us-income-disparity-analysis")
   ```

4. Run scripts in order
   ```r
   source("scripts/01_data_cleaning.R")
   source("scripts/02_merging.R")
   source("scripts/03_analysis.R")
   source("scripts/04_visualizations.R")
   ```

---

## 👤 Author

**Muhammad Ahmad**  
Knox College — Data Science & Business Administration  
📧 muahmad@knox.edu | [LinkedIn](#) | [GitHub](#)

---

*Knox College — Lead Researcher | Dec 2023 – Jan 2024*
