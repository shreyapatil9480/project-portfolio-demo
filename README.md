# Project Portfolio Demo

When do sales forecasts miss accuracy targets?

**Stakeholder:** Revenue Operations Analyst

## Key Insights

- Discounts above 20% degrade forecast accuracy in Q4.
- High seasonality regions need separate forecast models.
- West region forecasts are accurate 68% of the time at baseline.

## Dataset

Primary file: `data/sales_forecast.csv`  
Target variable: `forecast_accurate`

## Getting Started

```bash
pip install -r requirements.txt
jupyter notebook notebooks/case_study.ipynb
```


## CLI Usage

```bash
python src/train.py
python src/predict.py --input data/sample_input.csv
```

## Next Steps

**Done.** Docker training image and scheduled retraining workflow are implemented — see ### Implemented below.

---
*Analytics portfolio project — 2025-10*

<!-- build 7 -->

### Implemented

```bash
pip install -r requirements.txt
docker build -t train . && docker compose run train
```