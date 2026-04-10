# Simple Linear Regression — Study Hours vs Test Score

A beginner ML project predicting student test scores based on study hours using scikit-learn's LinearRegression. Built as part of my journey into machine learning.

---

## What it does

Takes a dataset of study hours and corresponding test scores, trains a simple linear regression model, and evaluates how well it generalizes on unseen data.

---

## Project Structure

```
├── lnr_reg.ipynb          # Main notebook
└── lnr_reg_practice.xlsx  # Dataset (71 samples)
```

---

## Workflow

1. **Load & inspect data** — 71 rows, no missing values
2. **Visualize** — scatter plot to confirm linear trend
3. **Split** — 75% train / 25% test (`random_state=43`)
4. **Train** — `sklearn.linear_model.LinearRegression`
5. **Evaluate** — MSE, MAE, R² on the test set

---

## Results

| Metric | Value |
|--------|-------|
| MSE | 0.69 |
| MAE | 0.69 |
| R² Score | **0.9975** |

The model fits the data extremely well, which makes sense given the near-perfect linear relationship between hours studied and scores.

---

## Tech Stack

- Python 3.14
- pandas, numpy, matplotlib
- scikit-learn

---

## How to Run

```bash
pip install pandas numpy matplotlib scikit-learn openpyxl
jupyter notebook lnr_reg.ipynb
```

> Make sure `lnr_reg_practice.xlsx` is in the same directory as the notebook.

---

## Key Takeaways

- Practiced the end-to-end ML pipeline: data loading → EDA → model training → evaluation
- Got comfortable reading performance metrics (MSE, MAE, R²)
- Linear regression works best when the relationship between variables is, well, linear and this dataset is a good example of that
