# Raw Dataset

## Source
**Lending Club Loan Data (2007–2020 Q3)**
- Kaggle: [ethon0426/lending-club-20072020q1](https://www.kaggle.com/datasets/ethon0426/lending-club-20072020q1)

## Details
| Property | Value |
|----------|-------|
| Rows | ~2,925,493 |
| Columns | 141 (31 selected for analysis) |
| Format | gzip-compressed CSV |
| File size | ~600 MB |

## How to Download

The raw dataset is too large for GitHub (>25 MB). To reproduce the analysis:

```python
import kagglehub

path = kagglehub.dataset_download("ethon0426/lending-club-20072020q1")
print("Downloaded to:", path)
```

A 100-row sample is included in `sample_100rows.csv` for reference.

## Important
- This file should **never** be edited directly
- All cleaning and transformations happen in `notebooks/02_cleaning.ipynb`
- Cleaned output is saved to `data/processed/`
