# Global Terrorism Data Analysis: Central America & The Caribbean (1970–2020)

## Project Overview
This repository contains a comprehensive, multi-phase data science and business intelligence project exploring regional terrorism trends from **1970 through 2020**. While utilizing the **Global Terrorism Database (GTD)**, this analysis specifically narrows its scope to examine the geopolitical shifts, incident frequencies, targeting strategies, and weapon profiles within **Central America and the Caribbean**.

The project scales from core exploratory data analysis to complex spatial-temporal mapping, concluding with enterprise-grade interactive dashboarding to translate raw numbers into actionable strategic insights.

---

## Repository Architecture

```text
📁 Global-Terrorism-Data-Analysis/
│
├── 📁 Phase-1-EDA/
│   ├── 📓 Phase 1 Code.ipynb                 # Python EDA & Trend Extraction
│   ├── 📄 Phase 1 Instructions.pdf           # Assignment Criteria
│   ├── 📄 Phase 1 Report.pdf                 # Documented Analytical Insights
│   ├── 📄 region_2.csv                       # Regional Dataset (Central America & Caribbean)
│   └── 📊 region_2_eda_subset.xlsx           # Extracted Subset with Pivot Tables & Charts
│
├── 📁 Phase-2-Geospatial-Analysis/
│   ├── 📓 Phase 2 Code.ipynb                 # Folium & GeoPandas Mapping Code
│   ├── 📄 Phase 2 Instructions.pdf           # Assignment Criteria
│   ├── 📄 Phase 2 Report.pdf                 # Spatial Analysis Documentation
│   ├── 📄 region_2.csv                       # Regional Dataset
│   ├── 🌐 terrorism_base_map.html            # Folium Incident Marker Map
│   ├── 🌐 terrorism_choropleth_map.html      # Folium Country Density Map
│   ├── 🌐 terrorism_heatmap.html             # Folium Spatial Intensity Map
│   └── 📄 world_countries.json               # GeoJSON Boundaries for Mapping
│
└── 📁 Phase-3-BI-Dashboards/
    ├── 📊 Global Terrorism Analysis Power BI.pbix  # Enterprise Power BI Dashboard
    ├── 📊 Global Terrorism Analysis Tableau.twbx   # Interactive Tableau Workbook
    ├── 📄 Phase 3 Instructions.pdf                 # Assignment Criteria
    ├── 📄 Phase 4 Report.pdf                       # Comprehensive Final Synthesis Report
    ├── 📄 Power BI Visualizations Report.pdf       # Power BI Screen Exports & Summaries
    ├── 📄 region_2.csv                             # Regional Dataset
    └── 📊 Tableau Visualizations PPT.pptx          # Dashboard Presentation Deck
```

## Phase Breakdowns

### 📊 Phase 1: Exploratory Data Analysis & Statistical Trends
* **Objective:** Clean, subset, and run preliminary temporal and categorical analysis on regional data spanning 50 years.
* **Key Tasks:**
  * Handled missing values, filtered out unconfirmed activities, and standardized data types via `pandas`.
  * Generated descriptive statistics to identify the most volatile years, dominant attack types, and heavily targeted sectors.
  * Exported an engineered subset (`region_2_eda_subset.xlsx`) equipped with targeted **Pivot Tables** and **Visual Charts** to track the evolution of incident frequencies.

### 🗺️ Phase 2: Geospatial & Spatial-Temporal Mapping
* **Objective:** Translate coordinates and geographic variables into visual risk surfaces and operational maps.
* **Key Tasks:**
  * Implemented `GeoPandas` and `Folium` in Python to convert latitude/longitude entries into spatial features.
  * Designed **three distinct interactive maps**:
    * *Base Map:* Individual localized incident pins with pop-up detailed metadata.
    * *Heatmap:* Density-based coordinate mapping to identify structural conflict hot zones.
    * *Choropleth Map:* Merged the regional attributes with a `world_countries.json` layer to visualize country-level aggregated metrics across the decades.

### 📈 Phase 3: Business Intelligence & Executive Dashboards
* **Objective:** Build enterprise-ready, cross-filtering analytical interfaces for non-technical stakeholders using Tableau and Power BI.
* **Key Tasks:**
  * **Tableau Architecture:** Created highly responsive dashboards emphasizing year-over-year growth metrics, weapon distribution, and multi-tier regional trend filtering.
  * **Power BI Architecture:** Engineered interactive reports utilizing DAX formatting, drill-down operational matrices, and comprehensive threat matrices.
  * **Final Synthesis:** Compiled a detailed final report translating visual dashboard metrics into actionable conclusions surrounding the long-term security landscape of the Central America and Caribbean regions.

---

## Core Technologies & Toolstack
* **Languages:** Python (Pandas, NumPy, GeoPandas, Folium, Matplotlib, Seaborn)
* **Environments:** Jupyter Notebook, VS Code
* **BI Software:** Tableau Desktop, Power BI Desktop
* **Data Management:** Microsoft Excel (Advanced Pivot Routing & Charting)
