# Iris Flower Classification

## Objective
Build a machine learning model that identifies the species of an iris flower (Setosa, Versicolor or Virginica) from its physical measurements.

## Dataset
Built-in Iris dataset from scikit-learn: 150 samples, 4 features (sepal length, sepal width, petal length, petal width) and 3 balanced classes (50 samples each). No missing values.

## Approach
1. Exploratory Data Analysis (shape, data types, null check, descriptive statistics)
2. Visualisation (pairplot, box plots, correlation heatmap)
3. Feature discussion
4. Train/test split (80/20, stratified, random_state=42)
5. Train three classifiers: Logistic Regression, KNN (k=5), Decision Tree
6. Evaluate with accuracy, classification report and confusion matrix
7. Confirm the ranking with 5-fold cross-validation

## Key Findings
- Petal length and petal width are the most discriminative features; sepal width is the least.
- Setosa is perfectly separable; all errors occur between Versicolor and Virginica.

## Results

| Model | Test accuracy | CV mean accuracy (5-fold) | CV std |
|---|---|---|---|
| Logistic Regression | 96.67% | 97.33% | 0.0249 |
| KNN (k=5) | 100.00% | 97.33% | 0.0249 |
| Decision Tree | 93.33% | 95.33% | 0.0340 |

## Best Model
**Logistic Regression.** It ties with KNN on cross-validation accuracy, but its result is consistent between the single split and cross-validation, and it is simpler and faster at prediction time. KNN's 100% on the single test split was partly due to that particular split.

## How to Run
Open `Iris_Classification.ipynb` in Google Colab or Jupyter Notebook and run all cells.
Required libraries: pandas, numpy, matplotlib, seaborn, scikit-learn.
