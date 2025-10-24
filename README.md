# Polynomial-Regression-Analysis-Notebook


## Overview
This notebook explores polynomial regression fits of varying degrees to noisy observations generated from a sine function. It demonstrates the concepts of underfitting, overfitting, and the bias-variance trade-off in polynomial regression.

## Purpose
The notebook aims to:
- Generate synthetic data from a sine function with added noise.
- Fit polynomial regression models of different degrees to the data.
- Visualize the fitted models compared to the true function and noisy observations.
- Analyze estimator performance through multiple simulations.
- Illustrate underfitting, overfitting, and calculate the root mean squared error for each model degree.

## Dataset
- Synthetic dataset with $$N = 20$$ observations.
- Input $$x$$ values are random samples in the interval $$[-1, 1]$$.
- Output $$y$$ values are generated from $$f(x) = \sin(x)$$ with added Gaussian noise of standard deviation 0.3.

## Methods
- Polynomial regression fits with degrees in $$$$ and extended range $$1$$ to $$15$$.[1]
- Use of NumPy's `polyfit` and `polyval` for polynomial parameter estimation and evaluation.
- Multiple simulations (100) to assess estimator variability.
- Plotting of true function $$f(x)$$, noisy observations, individual fits, average fits, and squared error.

## Results
- Visual comparison shows that lower degree polynomials (e.g., degree 1) underfit the data showing high bias.
- Higher degree polynomials (e.g., degree 10) overfit the observations, resulting in high variance.
- The plots highlight the trade-off between bias and variance across polynomial degrees.
- Root mean squared error is used to quantify the fit quality for each polynomial degree.

## Usage Instructions
1. Run all cells sequentially to generate synthetic data, fit models, perform simulations, and produce plots.
2. Modify noise level, number of observations, or polynomial degrees to explore different scenarios.
3. Use the plotting functions to visualize fitting and errors for customized data.

## Dependencies
- Python 3
- NumPy
- Matplotlib
