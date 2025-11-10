Solar Dataset EDA & Cleaning Project – Progress Update
Project Overview

This stage of the project focuses on performing end-to-end data profiling, cleaning, and exploratory data analysis (EDA) on the Benin Malanville solar dataset.
The goal at this stage is to clean and prepare the data for later comparison and region-ranking tasks.

All work up to this point has been implemented and committed to the repository.

✅ Progress Implemented and Committed

1. Data Loading

Loaded both raw and cleaned datasets in CSV format.

Used Pandas for efficient handling and exploration of the dataset.

2. Data Cleaning

Removed irrelevant column: Comments.

Replaced negative irradiance values (GHI, DNI, DHI) with zero to maintain realistic physical limits.

Detected and treated outliers in major columns (GHI, DNI, DHI, ModA, ModB, WS, WSgust) using Z-score analysis.

Outliers were either removed or imputed with the median value.

Exported the final cleaned dataset as data/benin_clean.csv for subsequent analysis.

3. Exploratory Data Analysis (EDA)

Summary Statistics: Generated descriptive statistics (count, mean, std, min, max, percentiles).

Missing Values Report: Identified and reported columns with more than 5% missing data.

Time Series Analysis: Visualized solar irradiance (GHI, DNI, DHI) over time and computed daily averages.

Hourly & Monthly Patterns: Analyzed how irradiance values vary across different hours of the day and months of the year.

Scatter & Bubble Plots: Explored relationships between GHI, temperature (Tamb), and relative humidity (RH) using scatter and bubble visualizations.

Correlation Heatmap: Displayed correlation relationships between key parameters such as GHI, DNI, DHI, ModA, ModB, Tamb, RH, WS, and WSgust.

Wind Analysis: Included both wind speed distribution histograms and a wind rose plot to visualize wind direction and strength patterns.

4. Cleaning Impact Analysis

Compared sensor readings (ModA & ModB) before and after cleaning to illustrate the effectiveness of the data cleaning process.

Visualized average readings pre- and post-cleaning using grouped bar plots.

5. Optimization for Large Dataset Performance

Handled performance challenges caused by the dataset’s large size (~525,000 rows).

Improved performance by:

Aggregating and resampling time series data (daily/hourly) for visualization.

Reducing redundant concatenations during summary and plotting steps.
