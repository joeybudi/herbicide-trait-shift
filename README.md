# Herbicide-trait shifts in seed sales

Mapping seed traits to herbicide systems and tracking each system's share of seed sales by state and year.

**Read it as a web page:** [https://joeybudi.github.io/projects/herbicide-trait-shift/](https://joeybudi.github.io/projects/herbicide-trait-shift/)

A small trait matrix maps every seed-trait code to the herbicide tolerances it carries. Sales are rolled up by state, crop, and year, and each herbicide system's share and year-over-year change are charted and mapped.

## Key results

- Every bag is classified into exactly one system, so stacked dicamba + 2,4-D traits are no longer double counted.
- Year-over-year change is computed within each state; the original lag compared across state boundaries.
- State maps show where dicamba-tolerant soybeans remain and how fast each state is shifting.

## What's in the notebook

- Trait-matrix join with validation
- Long-format rollups and correct shares
- Grouped year-over-year change
- State choropleths and trend lines

## About the data

All data in this repo is **simulated**. The original analysis ran on proprietary data, so this version keeps the methods and replaces the data and column names with realistic, generic stand-ins. The notebook generates its own data. The only download is public US Census boundary files for the maps.

## Run it

```bash
python -m venv .venv
source .venv/bin/activate      # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook herbicide_trait_shift.ipynb
```

The notebook is saved with its outputs, so you can also just open it on GitHub.

## Author

Joey Budi · [joeybudi.github.io](https://joeybudi.github.io) · [LinkedIn](https://www.linkedin.com/in/jbudi)
