# Gradient Descent for Linear Regression

This project demonstrates the implementation of Gradient Descent from scratch to fit a linear regression model on a synthetic dataset generated using `scikit-learn`. The notebook compares the analytical solution obtained from `scikit-learn`'s `LinearRegression` model against a manually implemented gradient descent approach.

---

## Overview

Linear regression attempts to model the relationship between a dependent variable $y$ and an independent variable $x$ by fitting a linear equation to observed data. The linear equation is defined as:

$$y = m \cdot x + b$$

Where:
- $m$ is the slope (coefficient)
- $b$ is the intercept

While standard machine learning libraries solve for parameters directly using normal equations, **Gradient Descent** is an iterative optimization algorithm used to minimize the loss function (Mean Squared Error) and find the optimal parameters.

---

## Dataset Description

The dataset is synthetically generated using `sklearn.datasets.make_regression` with the following parameters:
- **Number of samples:** 4
- **Number of features:** 1
- **Number of informative features:** 1
- **Target variables:** 1
- **Noise:** 80
- **Random State:** 13

---

## Implementation Steps

### 1. Dataset Generation & Visualization
- Generate a single-feature regression dataset.
- Scatter plot the generated data points using `matplotlib.pyplot`.

### 2. Analytical Linear Regression Model
- Fit a standard `LinearRegression` model from `sklearn.linear_model`.
- Extract the optimal intercept ($\hat{b}$) and coefficient ($\hat{m}$).
- Plot the fitted regression line against the scatter data.

### 3. Gradient Descent Optimization
- Set fixed or initial parameters for slope ($m$) and intercept ($b$).
- Compute predictions manually using $y_{pred} = m \cdot x + b$.
- Calculate gradients relative to the loss function to iteratively update $m$ and $b$ until convergence.

---

## Prerequisites & Dependencies

To run this notebook, ensure you have Python installed along with the following packages:

- `numpy`
- `matplotlib`
- `scikit-learn`

You can install all required dependencies via pip:

```bash
pip install numpy matplotlib scikit-learn
```
### Author: Engr. Abdul Muheet Ghouri
