Solar Dataset EDA & Cleaning Project
Project Overview

All tasks for the Benin Malanville solar dataset have been fully implemented and committed. The dataset is cleaned, analyzed, and ready for cross-country comparison and ranking.

✅ Progress Completed

1. Git & Environment Setup

Repository solar-challenge-week0 initialized.

Python virtual environment (venv) set up.

Branch setup-task created and merged into main.

Multiple commits made:

init: add .gitignore

chore: venv setup

ci: add GitHub Actions workflow

.gitignore configured to exclude data/ and temporary files.

requirements.txt created.

GitHub Actions workflow (.github/workflows/ci.yml) added to verify environment and dependencies.

README instructions for environment setup documented.

2. Data Profiling, Cleaning & EDA

Branch eda-benin created.

Notebook benin_eda.ipynb completed.

Raw and cleaned CSVs loaded using Pandas.

Summary statistics generated for all numeric columns.

Columns with >5% missing values identified.

Negative irradiance values (GHI, DNI, DHI) replaced with zero.

Outliers detected using Z-score for GHI, DNI, DHI, ModA, ModB, WS, WSgust; removed or imputed with median.

Cleaned dataset exported as data/benin_clean.csv.

Time series analysis of GHI, DNI, DHI performed; daily averages computed.

Hourly and monthly patterns visualized.

Scatter and bubble plots of GHI, Tamb, RH created.

Correlation heatmap of key variables completed.

Wind speed distribution and wind rose plots generated.

Cleaning impact analysis: pre- and post-cleaning ModA & ModB compared using grouped bar plots.

Performance optimization implemented for large dataset (~525,000 rows) with aggregation and reduced redundant operations.

3. Cross-Country Comparison

Branch compare-countries created.

Notebook compare_countries.ipynb completed.

Cleaned CSVs for Benin, Sierra Leone, and Togo loaded.

Boxplots for GHI, DNI, DHI across countries created.

Summary table of mean, median, and standard deviation for each metric generated.

Statistical testing (ANOVA/Kruskal–Wallis) performed for GHI; p-values reported.

Key observations documented: differences in median, variability, and averages highlighted.

Visual summary chart ranking countries by average GHI completed.

#. Highlights

Dataset fully cleaned and validated.

EDA visualizations complete (time series, scatter/bubble plots, wind rose, heatmaps).

Optimized for performance on large dataset.

Environment setup and CI workflow verified.

Project ready for further analysis and reporting.
