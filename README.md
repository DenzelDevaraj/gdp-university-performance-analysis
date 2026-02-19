# GDP & University Performance: A Global Analysis

## Project Overview
An investigation into the relationship between national economic conditions and university performance, using two real-world datasets: global GDP statistics (184 countries) and the World University Rankings (2,188 institutions). The project involved significant data wrangling to clean, standardise, and merge both datasets before conducting analysis across three core research questions.

## Tools & Technologies
- **Python (Google Colab)** - data cleaning, merging, and wrangling
- **Microsoft Excel** - pivot tables, scatter plots, and derived metrics
- **Libraries:** Pandas, NumPy

## Data Sources
- World GDP Dataset (Kaggle) — JSON format, 184 countries, 16 columns
- World University Rankings Dataset (Kaggle) — CSV format, 2,188 institutions, 14 columns

## Research Questions & Key Findings

**1. Do wealthier countries have higher-performing universities?**
Yes. A clear positive trend was identified — countries with high GDP per capita (e.g. Switzerland at $85,584, Ireland at $82,058) consistently hosted higher-scoring universities. Lower-income countries like India ($2,361) and Uganda ($735) clustered at the lower end of university scores. Analysis is correlational; causation was not assumed.

**2. Which countries punch above their weight in research influence relative to GDP?**
Smaller economies — particularly Cyprus, Uganda, and Lebanon — achieved the highest research influence per GDP dollar, outperforming major economies like the USA, China, and Germany on this metric. This suggests focused investment and academic policy can yield disproportionately strong research outcomes regardless of economic size.

**3. Is there a relationship between population density and university patent output?**
No clear relationship was found. Despite Taiwan showing high density and high patent output (avg 742 patents), Singapore — the densest country in the dataset at 8,240/km² — had only 26 average patents. A logarithmic scale was applied to the x-axis to better visualise the distribution. Patent output appears more closely tied to research funding and institutional priorities than population density.

## Data Wrangling Highlights
- Cleaned GDP columns containing symbols ($, Tn, Bn, %) and converted to floats
- Resolved country name mismatches between datasets (e.g. "USA" → "United States", "Slovak Republic" → "Slovakia")
- Handled Hong Kong's absence from the GDP dataset - dropped rather than merged with China to preserve data integrity
- Performed a left join merge on the standardised country column, preserving all 2,188 university records
- Imputed missing values in the broad_impact column using median substitution

## Files
- `Project_Final.ipynb` — Python code for data cleaning, wrangling, and merging
- `BUSAN_300_Project_Report.pdf` — Full written report including visualisations and analysis

## Skills Demonstrated
Data wrangling, dataset merging, exploratory data analysis, pivot table analysis, data visualisation, correlation analysis, analytical reasoning, Excel and Python integration
