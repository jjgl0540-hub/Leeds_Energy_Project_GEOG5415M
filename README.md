# Identifying Energy Vulnerability in Leeds Using Spatial Data Integration

This repository contains a spatial data analysis project developed for the GEOG5415M module.  
The project explores patterns of energy vulnerability across Leeds by integrating building energy efficiency data with selected socio-demographic indicators at the LSOA level.



## 1. Project Overview
This project develops a reproducible spatial data analysis workflow to examine variations in energy vulnerability across Leeds.  
Rather than relying solely on income-based indicators, the analysis integrates **Energy Performance Certificate (EPC)** data with census-derived characteristics to identify areas where structural housing conditions may exacerbate cold-related risks.

The analysis is intended as an **exploratory and decision-support exercise**, demonstrating how spatial data integration can inform more targeted energy and housing interventions.

**Intended audience:**
- Local policymakers and planners (for high-level spatial patterns and intervention prioritisation)
- Local government analysts and researchers (for statistically robust spatial analysis and clustering results)
- Students interested in applied spatial data analysis for public good

## 2. Data Sources

This analysis uses publicly available UK datasets:
- **Energy Performance Certificates (EPC, 2025)**
Domestic EPC records published by the UK Department for Housing and Communities Development (DLUHC).
These records are used to derive indicators of building energy efficiency.
- **Multiple Deprivation Index (IMD, 2019)**
Area-level socioeconomic deprivation indicator published by the UK Government using the 2011 LSOA framework.
- **LSOA Boundaries (2021)**
  LSOA area's boundary data sourced from the ONS Geoportal, used as the spatial reference framework for analysis.
  
All datasets have been aggregated or aligned to the LSOA level to ensure spatial consistency and avoid individual privacy issues.


## 3. Repository Structure
```
├── data/
│   └── raw/              #  (EPC 2025, IMD 2019, LSOA boundaries, ostcode-to-LSOA lookup)
├── outputs/
│   └── figures/          # Figures are exported from the notebook
├── notebook/
│   └── GEOG5415M_Final_Project_202018307.ipynb
└── README.md

```

## 4. Analysis Workflow
This notebook follows a structured spatial data science workflow:

1. Load and inspect datasets from multiple sources  
2. Perform data integrity and consistency checks  
3. Clean and standardise key variables  
4. Aggregate EPC records to the LSOA level  
5. Integrate EPC and IMD indicators  
6. Generate spatial and non-spatial visualisations

Key programming and data processing decisions are recorded in the notebook using Markdown cells.

## 5. How to Run the Analysis
To reproduce the analysis
1. Clone this repository
2. Install required Python packages
3. Open and run the notebook


## 6. Outputs

Running the notebook generates non-spatial distribution plots and spatial maps illustrating relative energy vulnerability across Leeds LSOAs.


## 7. Acknowledgement of Generative AI Use

This project made limited use of generative AI tools to support debugging and clarify Python syntax. All outputs are reviewed and adapted by the author.




