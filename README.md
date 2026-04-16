# malaysia-cost-of-living-eda

# Malaysia Cost of Living Analysis (2015–2022)

Exploratory data analysis of household income, expenditure, and inflation
trends across Malaysia's 16 states, using official DOSM survey data.

---

## Business questions

1. Which states face the highest affordability stress (expenditure relative to income)?
2. Has income growth kept pace with CPI inflation across states?
3. Which expenditure categories are driving cost of living increases?

---

## Data sources

| Dataset | Source | Years |
|---|---|---|
| Household Income & Expenditure Survey (HIES) | [open.dosm.gov.my](https://open.dosm.gov.my) | 2016, 2019, 2022 |
| Consumer Price Index (CPI) by state | [open.dosm.gov.my](https://open.dosm.gov.my) | 2015–2022 |
| Salaries & Wages Survey | [open.dosm.gov.my](https://open.dosm.gov.my) | 2015–2022 |

All raw files are stored in `/data/raw/` and are not modified.

---

## Key findings

1. **Affordability stress is highest in Sabah and Kelantan** — households
   in both states spend over 85% of median income on basic expenditure.
2. **Food CPI outpaced income growth in 11 of 16 states** between 2019–2022,
   with rural east Malaysian states hit hardest.
3. **KL and Selangor are outliers** — higher income, but housing costs
   consume a disproportionately larger share vs other states.

> Replace these with your actual findings once the analysis is complete.

---

## Methodology

- Data cleaning and merging: `01_data_cleaning.ipynb`
- Univariate distributions and trends: `02_univariate_analysis.ipynb`
- State-level comparisons and correlations: `03_bivariate_state_analysis.ipynb`
- Summary insights: `04_insights_summary.ipynb`

Engineered features:
- `affordability_ratio` = median expenditure / median income
- `real_income` = nominal income / CPI × 100

---

## Setup

```bash
git clone https://github.com/yourusername/malaysia-cost-of-living-eda
cd malaysia-cost-of-living-eda
pip install -r requirements.txt
```

Run notebooks in order (01 → 04) from the `/notebooks/` directory.

---

## Tools used

Python · pandas · numpy · matplotlib · seaborn · plotly · Jupyter

---

*Data sourced from the Department of Statistics Malaysia (DOSM).
This project is for portfolio and educational purposes.*
