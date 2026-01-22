---
title: "A Hybrid Minkowski-Log-Cosh Loss Function for Robust LSTM-Based Time Series Forecasting"
collection: publications
category: manuscripts
permalink: /publication/2025-hybrid-minkowski-log-cosh
excerpt: >
  We propose a Hybrid Minkowski–Log–Cosh (MLC) loss function for robust
  LSTM-based time series forecasting in noisy environments.
  The loss is defined as
  L(y,ŷ) = (1/N) ∑[log(cosh(yᵢ − ŷᵢ))]ᵖ,
  where the parameter p controls the trade-off between robustness to
  outliers and error sensitivity.
  Experiments on 11 years of malaria incidence data show a reduction in
  MAPE to 18.23% (vs. 20.96% with MSE) and approximately 117,000 fewer
  mispredicted cases under outlier contamination.
date: 2025-02-15
venue: 'IEEE Access'
paperurl: 'https://doi.org/10.1109/ACCESS.2025.3626795'
citation: 'Simsoba, K.-A., Oscar, N., & Mageto, T. (2025). A Hybrid Minkowski-Log-Cosh Loss Function for Robust LSTM-Based Time Series Forecasting. IEEE Access, 13, 187307–187319.'
mathjax: true
---

## Abstract

Robust learning is essential for time-series forecasting in real-world
settings where data are noisy, irregular, or contaminated by outliers.
This paper proposes a **Hybrid Minkowski–Log–Cosh (MLC) loss function**,
a tunable and theoretically grounded objective designed to improve the
stability and accuracy of **LSTM-based forecasting models**.

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

where $p > 0$ controls the robustness–sensitivity trade-off.

---

## Gradient Analysis

Let $\varepsilon_i = y_i - \hat{y}_i$.
The gradient with respect to $\hat{y}_i$ is

$$
\frac{\partial \mathcal{L}}{\partial \hat{y}_i}
=
-\,p
\left[\log\!\big(\cosh(\varepsilon_i)\big)\right]^{p-1}
\tanh(\varepsilon_i).
$$

This structure yields bounded gradients for large residuals, ensuring
stable optimization.

---

## Empirical Evaluation

The method was evaluated on **monthly malaria incidence data (2013–2023)**.

- **Clean data:** MAPE reduced to **18.23%**
- **Outlier regime:** ≈ **117,000 fewer mispredicted cases**
- **Complexity:** $\mathcal{O}(N)$, same as MSE and MAE

---

## How to Cite (APA)

Simsoba, K.-A., Oscar, N., & Mageto, T. (2025).  
*A Hybrid Minkowski-Log-Cosh Loss Function for Robust LSTM-Based Time Series Forecasting*.  
**IEEE Access, 13**, 187307–187319.  
https://doi.org/10.1109/ACCESS.2025.3626795
