---
title: "A Hybrid Minkowski-Log-Cosh Loss Function for Robust LSTM-Based Time Series Forecasting"
collection: publications
category: manuscripts
permalink: /publication/2025-hybrid-minkowski-log-cosh
excerpt: >
  We propose a Hybrid Minkowski–Log–Cosh (MLC) loss function for robust
  LSTM-based time series forecasting under noisy and outlier-contaminated
  conditions, validated on long-horizon public health data.
  How to cite: APA / IEEE / Harvard / Vancouver / BibTeX.
date: 2025-02-15
venue: 'IEEE Access'
paperurl: 'https://doi.org/10.1109/ACCESS.2025.3626795'
citation: 'Simsoba, K.-A., Oscar, N., & Mageto, T. (2025). A Hybrid Minkowski-Log-Cosh Loss Function for Robust LSTM-Based Time Series Forecasting. IEEE Access, 13, 187307–187319.'
mathjax: true
---

## Abstract

Robust learning is essential for time-series forecasting in real-world settings
where data are noisy, irregular, or contaminated by outliers. This paper proposes
a **Hybrid Minkowski–Log–Cosh (MLC) loss function**, a tunable and theoretically
grounded objective designed to improve the stability and accuracy of
**LSTM-based forecasting models**. The approach is validated on 11 years of
monthly malaria incidence data and consistently outperforms classical loss
functions under both clean and outlier-contaminated regimes.

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

This formulation yields smooth gradients for small residuals and suppresses the
influence of extreme errors, contributing to stable optimization.

---

## Empirical Evaluation

The proposed loss was evaluated using **LSTM models** on **monthly malaria
incidence data (2013–2023)**.

- **Clean data regime:**  
  MAPE reduced to **18.23%**, compared to **20.96%** under MSE.

- **Outlier-contaminated regime:**  
  Approximately **117,000 fewer mispredicted cases** relative to MSE.

- **Computational complexity:**  
  Training complexity remains $\mathcal{O}(N)$, matching standard regression
  losses.

---

## Key Contributions

- Novel hybrid loss function with tunable robustness  
- Explicit gradient-based analysis explaining stability  
- Improved forecasting accuracy on real public health data  
- Plug-and-play compatibility with LSTM and deep learning models  

---

## How to Cite

### APA
Simsoba, K.-A., Oscar, N., & Mageto, T. (2025).  
*A Hybrid Minkowski-Log-Cosh Loss Function for Robust LSTM-Based Time Series Forecasting*.  
**IEEE Access, 13**, 187307–187319.  
https://doi.org/10.1109/ACCESS.2025.3626795

---

### IEEE
K.-A. Simsoba, N. Oscar, and T. Mageto,  
“A Hybrid Minkowski-Log-Cosh Loss Function for Robust LSTM-Based Time Series Forecasting,”  
*IEEE Access*, vol. 13, pp. 187307–187319, 2025,  
doi:10.1109/ACCESS.2025.3626795.

---

### Harvard
Simsoba, K.-A., Oscar, N. and Mageto, T. (2025)  
‘A Hybrid Minkowski-Log-Cosh Loss Function for Robust LSTM-Based Time Series Forecasting’,  
*IEEE Access*, 13, pp. 187307–187319.  
doi:10.1109/ACCESS.2025.3626795.

---

### Vancouver
Simsoba K-A, Oscar N, Mageto T.  
A Hybrid Minkowski-Log-Cosh Loss Function for Robust LSTM-Based Time Series Forecasting.  
IEEE Access. 2025;13:187307–187319.  
doi:10.1109/ACCESS.2025.3626795.

---

### BibTeX
```bibtex
@article{Simsoba2025MLC,
  author  = {Simsoba, Kouyakou-Abalo and Oscar, Ngesa and Mageto, Thomas},
  title   = {A Hybrid Minkowski-Log-Cosh Loss Function for Robust LSTM-Based Time Series Forecasting},
  journal = {IEEE Access},
  volume  = {13},
  pages   = {187307--187319},
  year    = {2025},
  doi     = {10.1109/ACCESS.2025.3626795}
}
