---
title: "A Hybrid Minkowski-Log-Cosh Loss Function for Robust LSTM-Based Time Series Forecasting"
collection: publications
category: manuscripts
permalink: /publication/2025-hybrid-minkowski-log-cosh
excerpt: >
  This paper introduces a Hybrid Minkowski–Log–Cosh (MLC) loss function for
  robust LSTM-based time series forecasting under noisy and outlier-contaminated
  conditions. The proposed method provides a tunable trade-off between robustness
  and error sensitivity and is validated on long-horizon malaria incidence data,
  demonstrating improved accuracy and stability over standard loss functions.
date: 2025-02-15
venue: 'IEEE Access'
paperurl: 'https://doi.org/10.1109/ACCESS.2025.3626795'
citation: 'Simsoba, K.-A., Oscar, N., & Mageto, T. (2025). "A Hybrid Minkowski-Log-Cosh Loss Function for Robust LSTM-Based Time Series Forecasting." IEEE Access, 13, 187307–187319.'
mathjax: true
---

## Abstract

Robust learning is essential for time-series forecasting in real-world settings
where data are noisy, irregular, or contaminated by outliers. This paper proposes
a **Hybrid Minkowski–Log–Cosh (MLC) loss function**, a tunable and theoretically
grounded objective designed to improve the stability and accuracy of
**LSTM-based forecasting models**. The method is validated on long-horizon public
health data, with a particular focus on malaria incidence forecasting.

---

## Loss Function Definition

Let $y_i$ and $\hat{y}_i$ denote the true and predicted values at time $i$.
The proposed loss function is defined as

$$
\mathcal{L}(y,\hat{y})
=
\frac{1}{N}\sum_{i=1}^{N}
\left[\log\!\big(\cosh(y_i - \hat{y}_i)\big)\right]^p,
$$

where $p > 0$ is a Minkowski exponent controlling the trade-off between robustness
to outliers and sensitivity to prediction errors.

**Special cases**
- $p = 1$: Log-Cosh loss  
- $p \approx 2$: MSE-like behavior  
- $p < 2$: increased robustness to outliers  

---

## Gradient Analysis

Let $\varepsilon_i = y_i - \hat{y}_i$.  
The gradient with respect to the prediction $\hat{y}_i$ is

$$
\frac{\partial \mathcal{L}}{\partial \hat{y}_i}
=
-\,p
\left[\log\!\big(\cosh(\varepsilon_i)\big)\right]^{p-1}
\tanh(\varepsilon_i).
$$

This formulation yields smooth gradients for small residuals and naturally
suppresses the influence of extreme errors, contributing to stable optimization.

---

## Empirical Evaluation

The proposed loss was evaluated using **LSTM models** on **monthly malaria
incidence data (2013–2023)**.

- **Clean data regime:**  
  MAPE reduced to **18.23%**, compared to **20.96%** under MSE.

- **Outlier-contaminated regime:**  
  Approximately **117,000 fewer mispredicted cases** relative to MSE.

- **Computational efficiency:**  
  Training complexity remains $\mathcal{O}(N)$, matching standard regression
  losses.

---

## Key Contributions

- Novel hybrid loss function with tunable robustness  
- Explicit gradient analysis explaining optimization stability  
- Improved forecasting accuracy on real public health data  
- Plug-and-play compatibility with LSTM and deep learning models  

---

[Access the full paper here](https://doi.org/10.1109/ACCESS.2025.3626795)
