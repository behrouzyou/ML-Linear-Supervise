# Auto MPG Prediction — Machine Learning

A Machine Learning regression project that predicts a vehicle's fuel efficiency (Miles Per Gallon) using vehicle specifications and compares multiple regression techniques.

## Project Overview

The goal of this project is to explore the relationship between vehicle characteristics and fuel efficiency, train regression models, evaluate their performance, and analyze prediction errors through residual diagnostics.

## Dataset

The project uses the **Auto MPG** dataset.

- **Target variable:** `mpg` — Miles Per Gallon
- **Input features:**
  - `weight`
  - `displacement`
  - `horsepower`
  - `cylinders`
  - `model year`

### Data Preprocessing
- Handle missing values represented by `?`.
- Convert `horsepower` to a numeric data type.
- Remove rows containing missing values.
- Drop the `car name` column.
- Split the dataset into training and testing sets (80/20).

## Machine Learning Models

The project implements and compares the following regression approaches:

1. **Simple Linear Regression** — Predicting MPG using vehicle weight.
2. **Polynomial Regression** — Capturing nonlinear relationships using polynomial features.
3. **Multiple Linear Regression** — Predicting MPG using multiple vehicle characteristics.
4. **Ridge Regression (L2)** — Applying regularization to control model complexity.
5. **Lasso Regression (L1)** — Regularization with feature coefficient shrinkage.
6. **Elastic Net** — Combining L1 and L2 regularization.
7. **Ridge Regression with Feature Interaction** — Adding an interaction between vehicle weight and model year.

## Evaluation Metrics

Model performance is evaluated using:

- **RMSE (Root Mean Squared Error):** Measures the typical magnitude of prediction errors, with greater penalties for larger errors.
- **R² Score (Coefficient of Determination):** Measures how much of the target variance is explained by the model.

Training and testing errors are compared to help assess generalization.

## Exploratory Data Analysis

The notebook includes:

- Descriptive statistics and MPG distribution.
- Correlation analysis and a correlation heatmap.
- Scatter plots of MPG against vehicle features.
- Actual vs. predicted value visualization.
- Residual analysis and residual distribution plots.
- Q-Q plots for examining residual normality.
- Residual comparisons against weight and model year.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- SciPy
- Jupyter Notebook

## Installation

Clone the repository:

```bash
git clone https://github.com/behrouzyou/ML-Linear-Supervise.git
```

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn scipy jupyter
```

Place `auto-mpg.csv` in the same directory as the notebook, then launch Jupyter:

```bash
jupyter notebook
```

Open `auto-mpg-ml.ipynb` and run the cells.

## Project Structure

```text
auto-mpg-ml/
├── auto-mpg-ml.ipynb
├── auto-mpg.csv
└── README.md
```

## Key Learning Objectives

- Understand regression algorithms and their differences.
- Explore feature relationships using statistical analysis and visualization.
- Apply regularization techniques to linear models.
- Engineer interaction features to capture additional relationships.
- Evaluate regression performance using appropriate metrics.
- Diagnose model errors using residual analysis.

## Future Improvements

- Compare all models in a single evaluation table.
- Use cross-validation and hyperparameter tuning.
- Experiment with additional regression algorithms.
- Investigate feature scaling and feature selection.
- Improve generalization through systematic model comparison.

## Author

**Behrouz**

GitHub: [@behrouzyou](https://github.com/behrouzyou)

---

*This project is part of my Machine Learning learning journey, with a focus on regression, feature engineering, model evaluation, and statistical diagnostics.*