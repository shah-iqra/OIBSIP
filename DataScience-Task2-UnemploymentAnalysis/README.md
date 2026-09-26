# Unemployment Analysis in India

## Objective
Analyse regional and temporal trends in India's unemployment rate, with a focus on the impact of the COVID-19 pandemic on unemployment, employment, and labour participation.

## Dataset
Unemployment in India (Kaggle) — 267 records covering 26 Indian states/union territories from January 2020 to October 2020. Includes Estimated Unemployment Rate (%), Estimated Employed, Estimated Labour Participation Rate (%), Region, and Zone.

## Approach
1. Data cleaning (Date conversion to datetime, column renaming, null/duplicate check)
2. Exploratory Data Analysis (region-wise averages, unique regions/zones, date range)
3. Region-wise average unemployment rate (bar chart)
4. Month-wise unemployment trend (all-India line chart)
5. State-level trend comparison (Haryana, Uttar Pradesh, Maharashtra)
6. Top 10 states by average unemployment rate
7. Correlation heatmap (unemployment rate, employment, labour participation)
8. Pre-COVID vs Post-COVID comparison (Jan-Feb 2020 vs Mar-Oct 2020)

## Key Findings
- The all-India unemployment rate spiked sharply to nearly 24% in April 2020, aligning with India's nationwide COVID-19 lockdown (started 25 March 2020), then gradually declined through October 2020.
- Haryana had the highest average unemployment rate (27.47%), while Meghalaya, Sikkim, and Uttar Pradesh had the lowest averages.
- Uttar Pradesh showed the sharpest single-month spike (close to 45% in April 2020) despite a low overall average — showing that "high average" and "high volatility" are different patterns.
- Average unemployment rate rose from 9.23% (pre-COVID) to 12.98% (post-COVID), while average labour participation rate fell from 44.44% to 41.02%.
- Employment count and labour participation rate are strongly correlated (0.85); unemployment rate is more independent, driven by external shocks like the lockdown.

## Recommendations
1. States with persistently high unemployment (Haryana, Tripura, Jharkhand, Bihar) may need long-term employment programs, not just pandemic relief.
2. States with sharp but short-lived spikes (Uttar Pradesh) may benefit from emergency income-support programs during future shocks.
3. Policies should also address workforce re-entry, since the drop in labour participation suggests some people left the workforce entirely during the lockdown.

## Limitation
The dataset only covers January–October 2020, so there is no pre-2020 baseline for comparison, and it's unclear whether unemployment fully recovered after October 2020.

## Tools & Technologies
Python, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook

## How to Run
Open `Unemployment_Analysis.ipynb` in Google Colab or Jupyter Notebook and run all cells. Requires the "Unemployment_Rate_upto_11_2020.csv" file (from Kaggle: "Unemployment in India" dataset) to be uploaded to the same environment.
