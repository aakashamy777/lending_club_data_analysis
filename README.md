# Lending Club Loan Default Analysis

**Sector:** Finance | **Dataset:** Lending Club 2007–2020 Q3 | **Rows:** 2.9M

---

## Problem Statement

What borrower, loan, and geographic factors drive loan default rates across 13 years of US peer-to-peer lending?

LendingClub is the world's largest peer-to-peer lending platform, with $15.98 billion in loans originated through December 2015. Understanding what drives loan defaults is critical for risk management, credit pricing, and borrower assessment.

## Key Findings

| KPI | Value |
|-----|-------|
| Overall Default Rate | 13.08% |
| Peak Default Year | 2007 (26%) — financial crisis |
| Highest Default Grade | G (≈45%) vs A (≈4%) |
| Strongest Predictor | Interest rate (correlation = +0.21) |
| Logistic Regression ROC-AUC | 0.6887 |

## Folder Structure

```
lending_club_data_analysis/
├── README.md                  ← You are here
├── data/
│   ├── raw/                   ← Original dataset info & sample
│   └── processed/             ← Cleaned CSVs & Tableau exports
├── docs/
│   └── data_dictionary.md     ← Column descriptions & definitions
├── notebooks/
│   ├── 01_data_loading.ipynb          ← Download & initial load
│   ├── 02_cleaning.ipynb              ← Full ETL pipeline
│   ├── 03_eda.ipynb                   ← Exploratory data analysis
│   ├── 04_statistical_analysis.ipynb  ← T-tests, chi-square, logistic regression
│   └── 05_final_load_prep.ipynb       ← Tableau export preparation
└── tableau/
    ├── dashboard_links.md     ← Tableau Public URL
    └── screenshots/           ← EDA charts & dashboard screenshots
```

## Dataset

- **Source:** [Kaggle — Lending Club 2007–2020 Q3](https://www.kaggle.com/datasets/ethon0426/lending-club-20072020q1)
- **Size:** 2,925,493 rows × 31 selected columns
- **Format:** gzip-compressed CSV
- **Issues addressed:** Missing values, inconsistent formats, percentage strings, date parsing, outlier capping

## Tools & Technologies

| Tool | Purpose |
|------|---------|
| Python (pandas) | ETL pipeline, data cleaning |
| scipy | Statistical hypothesis testing |
| scikit-learn | Logistic regression, ROC-AUC |
| matplotlib / seaborn | EDA visualisations |
| Tableau Public | Interactive dashboard |
| GitHub | Version control & collaboration |

## Dashboard

📊 **Tableau Public URL:** [To be added after publishing]

## How to Reproduce

1. Clone this repository
2. Run `notebooks/01_data_loading.ipynb` to download the dataset via kagglehub
3. Run notebooks 02 through 05 in order
4. Open the Tableau dashboard via the URL in `tableau/dashboard_links.md`
