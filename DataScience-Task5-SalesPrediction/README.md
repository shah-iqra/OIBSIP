# Sales Prediction Using Advertising Data

## Objective
Build a regression model that predicts product sales based on advertising spend across TV, Radio and Newspaper channels.

## Dataset
Advertising.csv — 200 records with TV, Radio and Newspaper advertising budgets and resulting Sales. No missing values.

## Approach
1. Exploratory Data Analysis (shape, data types, null check, descriptive statistics)
2. Visualisation (pairplot, individual scatter plots, correlation heatmap)
3. Train/test split (80/20)
4. Train two regression models: Linear Regression (baseline), Random Forest Regressor
5. Evaluate with MAE, RMSE and R²
6. Actual vs Predicted plot, residual plot
7. Feature importance / coefficient analysis

## Key Findings
- TV advertising has the strongest relationship with sales, followed by Radio.
- Newspaper advertising has almost no measurable effect on sales.
- The true relationship is not fully linear, likely due to interaction effects between channels.

## Results

| Model | MAE | RMSE | R² |
|---|---|---|---|
| Linear Regression | 1.46 | 1.78 | 0.90 |
| Random Forest | 0.62 | 0.76 | 0.98 |

## Best Model
**Random Forest Regressor.** It outperforms Linear Regression on all three metrics, suggesting the relationship between advertising spend and sales includes non-linear or interaction effects that Random Forest captures but Linear Regression cannot.

## Business Recommendation
Focus investment on TV advertising, use Radio strategically to complement it, and consider reducing Newspaper spend given its minimal measurable impact.

## Limitation
The dataset is small (200 samples) and does not account for seasonality, competitor activity, or long-term brand effects.

## How to Run
Open `Sales_Prediction.ipynb` in Google Colab or Jupyter Notebook and run all cells.
Required libraries: pandas, numpy, matplotlib, seaborn, scikit-learn.
