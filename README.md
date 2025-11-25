# ECO225 – Decoding Airbnb Pricing in Boston:How hosts, properties, and locations shape costs for users.  
*University of Toronto – Big Data Tools for Economists*

## Project Overview
This project investigates the following research question:

### **“In what ways do host attributes, property type, and location contribute to the pricing structure of Airbnb listings in Boston?”**

Using Airbnb listings data combined with Boston neighborhood socioeconomic indicators, this project applies:

- Data cleaning & merging  
- Exploratory data visualization
- Web scrapping
- OLS regressions (baseline → expanded → fixed effects → non-linear)  
- Decision trees  
- Random forest models  
- Economic interpretation & policy implications  

All main results are documented in the final research paper.

---

## Files in This Repository

### ** 1. Research Output (Final Paper)**
- **Final Paper:** [`final_paper.pdf`](final_paper.pdf)

---

### ** 2. Code and Analysis**
- **Python Notebook:** [`final_project.ipynb`](final_project.ipynb)  
- **Notebook PDF Export:** [`final_project.pdf`](final_project.pdf)

---

### ** 3. Datasets Used**
- **Airbnb Listings:** [`listings.csv`](listings.csv)  
- **Neighborhood Tables:** [`2015-2019_neighborhood_tables_2021.12.21.xlsm`](2015-2019_neighborhood_tables_2021.12.21.xlsm)  
- **Calendar / Availability:** [`calendar.csv`](calendar.csv)

---

## Key Findings

### 1. Location is the strongest predictor  
Neighborhood income, poverty rate, and region consistently explain the majority of price differences.  
Higher-income areas (e.g., Back Bay, Beacon Hill) have significantly higher prices.

### 2. Property characteristics matter  
- Each additional **bedroom** → approx. **+$69**  
- Each additional **bathroom** → approx. **+$24**  
(OLS Table 1 & 2)

### 3. Host attributes have limited influence  
- **Superhost status** is *not significant* in most OLS models  
- Number of listings matters only in machine learning models  
- Host experience contributes modestly

### 4. Pricing is non-linear  
- Income has diminishing returns  
- Random Forest confirms threshold effects  
- Decision tree splits first on **income**, then **region**

---

## Methods Used
- Python (pandas, numpy, seaborn, matplotlib, statsmodels)
- Decision Trees & Random Forest (sklearn)
- Geospatial mapping with OSMnx + GeoPandas
- Web Scrappings
- Econometric modeling (OLS, fixed effects, nonlinear specs)

---
