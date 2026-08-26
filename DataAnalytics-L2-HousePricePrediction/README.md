# House Price Prediction with Linear Regression

This project completes **Level 2 — Task 1** using the public [Housing Prices Dataset on Kaggle](https://www.kaggle.com/datasets/yasserh/housing-prices-dataset).

## Files

- `House_Price_Prediction_Linear_Regression.ipynb` — complete, executed analysis notebook
- `Housing.csv` — Kaggle source data used by the notebook
- `requirements.txt` — Python dependencies
- `screenshots/` — project summary, completed checklist, and all five analytical charts

## Model results

| Model | MSE | RMSE | R² |
|---|---:|---:|---:|
| Linear Regression | 1,754,318,687,330.67 | 1,324,506.96 | 0.6529 |
| Ridge Regression | 1,778,832,738,127.60 | 1,333,728.88 | 0.6481 |

Linear Regression performed slightly better than Ridge on the fixed 20% test set. The baseline explains about **65.3%** of the observed variation in test-set prices.

## Run locally

1. Keep `Housing.csv` in the same folder as the notebook.
2. Install dependencies with `pip install -r requirements.txt`.
3. Open the notebook in Jupyter or VS Code and select a Python kernel.
4. Run all cells from top to bottom.

The notebook includes a Kaggle download fallback if the local CSV is missing.

## Scope note

The selected Kaggle dataset contains a broad preferred-area indicator (`prefarea`) but does not include exact neighborhood or property age. Those unavailable fields are documented instead of being fabricated.
