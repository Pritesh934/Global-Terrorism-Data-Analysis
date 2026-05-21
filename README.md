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

### 📈 Phase 3: Business Intelligence & Dashboards
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

## Key Phase Wise Results & Analytical Insights

### 📊 Phase 1: Temporal Trends & Categorical Profiles
* **Peak of Volatility:** The analysis identified a massive surge in regional conflict during the late 1970s, peaking dramatically in **1980** with **over 1,300 recorded incidents** in a single year, followed by a secondary sustained wave of activity throughout the late 1980s. 
* **Targeting Strategies:** The private sector, citizens, property, and military/government installations emerged as the most heavily targeted entities.
* **Tactical Profiling:** **Facility/Infrastructure Attacks** and **Armed Assaults** dominated the categorical distribution, with **Firearms** and **Explosives** standing as the primary weapon types utilized across the 50-year timeframe.

### 🗺️ Phase 2: Spatial Hot Zones & Geographic Clustering
* **Primary Regional Hotspots:** Spatial coordinate mapping via Folium revealed dense operational clusters heavily concentrated in **El Salvador**, **Guatemala**, and **Nicaragua**, tracking closely with the historical timelines of civil conflicts in those nations.
* **Macroscopic Density (Choropleth):** Integrating country boundary layers (`world_countries.json`) confirmed that **El Salvador** sustained the highest aggregate density of tracking data points in the Central American region over the 1970–2020 window.
* **Microscopic Intensity (Heatmap):** Density-based heat mapping pinpointed specific urban capital areas (e.g., **San Salvador** and **Guatemala City**) as high-intensity structural risk zones, contrasting against more dispersed incidents in rural border territories.

### 📈 Phase 3: Strategic Dashboards & Portfolio Visualizations
* **Tableau Interactive Architecture:** Developed dynamic, multi-tier filtering dashboards that reveal a significant, steady decline in macro-regional terrorist activity starting in the mid-1990s through 2020. This allows viewers to interactively cross-filter weapon types against specific country casualty counts.
* **Power BI Intelligence System:** Implemented advanced data modeling and DAX measures to calculate year-over-year percentage variances, highlighting operational threat matrix shifts where infrastructure-targeted attacks gradually eclipsed armed assaults in the project’s later decades.
* **Deliverables:** Produced formal presentation decks and executive summaries demonstrating how business intelligence software effectively converts messy spatial-temporal event rows into clear risk-assessment maps for global stakeholders.

## 🛠️ Repository Reproducibility & Local Setup
This repository is engineered to be fully modular and self-contained. To ensure absolute reproducibility, a local copy of the regional dataset (`region_2.csv`) is explicitly packaged inside *every* phase subfolder so each phase can be executed independently.

### Quick Start:
1. Clone the repository:
   ```bash
   git clone [https://github.com/Priteshdas9/global-terrorism-data-analysis.git](https://github.com/Priteshdas9/global-terrorism-data-analysis.git)
