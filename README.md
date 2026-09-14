# CESI Health Project

This folder contains the current analysis code and exported data for the county-level CESI and health project. 

## Code order

1. `00_construct_cesi_scores.Rmd`: creating Practice and Meaning CESI.
2. `01_prepare_health_outcomes.Rmd`: clean and merge data from CDC PLACES and County Health Rankings & Roadmaps.
3. `02_construct_adversity_score.Rmd`: constructs the county adversity score.
4. `03_primary_health_models.Rmd`: multillevel model M1 and M2 nesting county within state.
5. `04_sensitivity_analyses.Rmd`: additional analysis for correlations, linear regression, state fixed-effects, within/between-state, both-CESI in the same model, four adversity-domain, and interaction models.
6. `05_tables_and_figures.Rmd`: create tables and figures.

## Folder contents

- `code/`: current scripts 00–05
- `data/raw/`: source files needed for 00–03
- `data/derived/`: constructed CESI, health, adversity index
- `output/primary_health_models/`: primary MLM estimates and model checks
- `output/sensitivity_analyses/`: geographic and model-specification checks
- `output/tables_and_figures/`: table and figures

`data/derived/health_analysis/county_health_analysis_long.csv` is the master file and contains the health outcomes, both CESI measures, adversity measures, baseline covariates, county and state identifiers.
