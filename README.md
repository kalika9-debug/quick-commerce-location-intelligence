# Quick-Commerce Location Intelligence & Expansion Strategy

> A geospatial decision-support system for identifying high-potential dark-store expansion locations across India.

## Overview

Quick-commerce expansion is not simply about finding high-demand cities. A market can have strong demand but still be unattractive due to **high competition, store saturation, or limited competitive whitespace**.

This project analyzes the observed networks of **Blinkit, Zepto, and Swiggy Instamart** to answer:

> **Where should a quick-commerce brand expand next?**

The system combines **demand, competition, brand strength, store density, and geospatial intelligence** to identify and evaluate expansion opportunities.

---

## Project Snapshot

| Metric | Scale |
|---|---:|
| Dark Stores Analyzed | **4,081** |
| Brands | **3** |
| Decision-Ready Locations | **3,232** |
| Markets Evaluated | **48** |
| Expansion Markets | **12** |
| Final Output | **Interactive Location Intelligence Engine** |

---

## Tech Stack

`Python` `Pandas` `NumPy` `GeoPandas` `OpenStreetMap` `Plotly` `Jupyter Notebook` `Geospatial Analytics`

---

## Methodology

The project follows an end-to-end location intelligence workflow:

**Market Network → Demand Intelligence → Competition Analysis → Opportunity Engineering → Scoring → Expansion Strategy → Interactive Site Evaluation**

### Demand Intelligence
A **Retail Demand Index (RDI)** was used to measure market quality beyond population alone.

### Competition Intelligence
Competitive pressure was evaluated using **competitor presence, brand share, store density, and local whitespace**.

### Opportunity Scoring
Each location received a **Location Opportunity Score / 100** based on:

- **40%** Demand Strength
- **20%** Competition Opportunity
- **15%** Competitor Pressure
- **15%** Local Brand Strength
- **10%** Density Opportunity

---

## Key Results

From **48 evaluated markets**:

| Strategy | Markets |
|---|---:|
| 🟢 EXPAND | **12** |
| 🟡 WATCH | **12** |
| ⚪ LOW PRIORITY | **24** |

**Coimbatore** ranked as the strongest baseline opportunity, while **Madurai** demonstrated strong ranking stability.

### Key Insight

> **High demand does not automatically mean high expansion potential. The real opportunity lies where demand remains strong without excessive competitive pressure.**

---

## Interactive Location Intelligence Engine

The final notebook converts the analysis into an interactive site-screening system.

### Input
- Indian city/town or coordinates
- Candidate brand
- Search radius

### Output
- Preliminary Site Score / 100
- Demand Strength
- Market Opportunity
- Nearby Dark Stores
- Competitor Count
- Competitive Whitespace
- Expansion Strategy
- Model Reliability
- Local Competitive Landscape

---

## Case Study — Pachora, Maharashtra

**Brand:** Blinkit  
**Site Score:** **84.4 / 100**  
**Recommendation:** 🟢 **Strong Expansion Candidate**

The model detected **0 mapped competitors within 5 km and 100% competitive whitespace**, indicating potential first-mover opportunity.

However, the demand intelligence uses Nashik as the nearest reference market, so further local validation is required.

**Outcome:** High-potential candidate for detailed feasibility analysis.

---

## Case Study — Mumbai, Maharashtra

**Brand:** Swiggy Instamart  
**Site Score:** **67.7 / 100**  
**Recommendation:** 🟡 **Consider / Watch**

Mumbai showed strong demand (**0.88**), but the selected 5 km catchment contained **37 dark stores and 28 competitors**, resulting in a **76% competitor ratio** and only **24% competitive whitespace**.

**Outcome:** Attractive demand, but high competitive pressure increases expansion risk.

---

## Repository Structure

```text
quick-commerce-location-intelligence/
│
├── Notebooks/
│   ├── 01_data_ingestion.ipynb
│   ├── 02_Data_Cleaning_&_Validation.ipynb
│   ├── 03_Exploratory_Data_Analysis_(EDA).ipynb
│   ├── 04_Census_Analysis_and_Retail_Demand_Index.ipynb
│   ├── 05_OpenStreetMap_Feature_Extraction.ipynb
│   ├── 06_Feature_Engineering.ipynb
│   ├── 07_Location_Opportunity_Engineering.ipynb
│   ├── 08_Location_Opportunity_Scoring_Model.ipynb
│   ├── 09_Market_Segmentation_&_Expansion_Strategy.ipynb
│   └── 10_Interactive_Location_Intelligence_Engine.ipynb
│
├── Reports/
│   └── Project documentation and executive summary
│
├── dataset/
│   └── Project datasets
│
├── output/
│   └── Analysis outputs and model results
│
├── presentation/
│   └── Project presentation
│
└── README.md
```

---

## Business Value

The project transforms:

**4,081 dark stores → 3,232 scored locations → 48 evaluated markets → 12 expansion priorities → site-level recommendations**

It provides a structured framework for **market screening, competitive analysis, whitespace identification, and candidate-site evaluation**.

---

## Limitations

The model provides **strategic site-screening intelligence**, not guaranteed profitability.

Final expansion decisions should additionally consider:

- Actual order demand
- Property rent
- Delivery economics
- Rider availability
- Traffic and accessibility
- Operating costs
- Real-time competitor activity

---

## Conclusion

Instead of asking:

> **Where is demand highest?**

this project asks the more useful business question:

> ### **Where is commercially attractive demand still available?**

The result is an end-to-end **quick-commerce location intelligence system** that turns raw geospatial data into actionable expansion recommendations.
