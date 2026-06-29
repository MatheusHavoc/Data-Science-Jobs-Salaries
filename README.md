# Data Science Jobs Salaries

Professional Python project for salary analytics in data roles. The original notebook is preserved and reusable pipeline code now lives in `src/salary_analysis/`.

## Staff Data Engineer assessment

This is a supporting portfolio project. It demonstrates descriptive analytics and business-question framing, but it is less engineering-heavy than the data-quality and modeling projects. The new structure makes it easier to run, test and extend.

## How to run

```bash
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
python -m pytest
python -m salary_analysis.pipeline --input data/raw/ds_salaries.csv --output data/processed
```

## Project structure

- `Data_Science_Jobs_Salaries.ipynb`: original analysis.
- `src/salary_analysis/`: reusable Python pipeline.
- `tests/`: ingestion and data-quality tests.
- `data/`: raw and processed file locations.

## Current limitations

- The raw dataset is not committed.
- Analytical aggregations from the notebook should be moved into typed functions.
- A SQL version of the main aggregations would improve the Analytics Engineering signal.
