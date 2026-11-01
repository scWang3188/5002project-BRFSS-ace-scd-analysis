# BRFSS 2023: ACEs and Subjective Cognitive Decline — Descriptive Statistics & EDA

CityU 5002 group project. This repository contains Member B's descriptive
statistics and exploratory data analysis (Table 1 + Figures 1–7) for the
association between Adverse Childhood Experiences (ACEs) and Subjective
Cognitive Decline (SCD) in BRFSS 2023 (age ≥ 45, 10 states).

## Folder structure

- `notebooks/02_Descriptive_EDA.ipynb` — main analysis notebook (survey-weighted Table 1 + all figures)
- `figures/` — exported figures (Fig 1–7, PNG)
- `tables/Table1_characteristics_by_SCD.csv` — weighted Table 1 by SCD status

## Data & run order

1. Run `01_..._Preprocessing` (Member A) to produce the analysis CSV
2. Run `notebooks/02_Descriptive_EDA.ipynb` — expects the preprocessed CSV in the working directory

## Methods notes

- Complex survey design: `_LLCPWT` weights, `_STSTR` strata, `_PSU` PSU;
  Taylor linearization SEs; design-based Wald chi-square tests
- Table 1: unweighted n + weighted %, P from design-adjusted chi-square