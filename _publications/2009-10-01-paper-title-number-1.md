---
title: "A Hybrid Minkowski-Log-Cosh Loss Function for Robust LSTM-Based Time Series Forecasting"
collection: publications
category: manuscripts
permalink: /publication/2025-hybrid-minkowski-log-cosh
excerpt: >
  This research introduces a novel Hybrid Minkowski–Log–Cosh (MLC) loss function for robust LSTM-based time series forecasting in noisy environments. The loss function, defined as $\mathcal{L}(y,\hat{y}) = \frac{1}{N}\sum_{i=1}^{N} [\log(\cosh(y_i - \hat{y}_i))]^p$, provides a tunable framework where parameter $p$ controls the trade-off between outlier robustness and error sensitivity. Validated on 11 years of malaria incidence data, MLC achieves 18.23% MAPE (vs. 20.96% for MSE) in clean data regimes and reduces mispredicted cases by approximately 117,000 in outlier-contaminated scenarios. The method maintains $\mathcal{O}(N)$ computational complexity while offering explicit gradient analysis and plug-and-play compatibility with deep learning models.
date: 2025-02-15
venue: 'IEEE Access'
paperurl: 'https://doi.org/10.1109/ACCESS.2025.3626795'
citation: 'Simsoba, K.-A., Oscar, N., & Mageto, T. (2025). "A Hybrid Minkowski-Log-Cosh Loss Function for Robust LSTM-Based Time Series Forecasting." IEEE Access, 13, 187307–187319.'
mathjax: true
---

## Abstract

Robust learning is essential for time-series forecasting in real-world settings where data are noisy, irregular, or contaminated by outliers. This paper proposes a **Hybrid Minkowski–Log–Cosh (MLC) loss function**, a tunable and theoretically grounded objective designed to improve the stability and accuracy of **LSTM-based forecasting models**. The method is validated on long-horizon public health data, with a particular focus on malaria incidence forecasting.

---

## Loss Function Definition

Let $y_i$ and $\hat{y}_i$ denote the true and predicted values at time $i$.
The proposed loss is defined as

$$
\mathcal{L}(y,\hat{y})
=
\frac{1}{N}\sum_{i=1}^{N}
\left[\log\!\big(\cosh(y_i - \hat{y}_i)\big)\right]^p
$$

where $p > 0$ is a tunable Minkowski exponent controlling the trade-off
between robustness to outliers and error sensitivity.

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
\tanh(\varepsilon_i)
$$

This formulation yields smooth gradients for small residuals and naturally
suppresses the influence of extreme errors.

---

## Empirical Evaluation

The loss was evaluated using **LSTM models** on **11 years (2013–2023)**
of monthly malaria incidence data.

### Clean data regime (best $p = 2.25$)
- **MAE:** 2,515.38
- **MAPE:** 18.23% (down from 20.96% with MSE)
- **RMSE:** 3,671.74
- Faster convergence than MSE, MAE, and Log-Cosh

### Noisy / outlier-contaminated regime (best $p = 1.5$)
- **MAE:** 3,676.36
- **Median AE:** 2,192.06
- **SMAPE:** 24.63%
- Approximately **117,000 fewer mispredicted cases** compared to MSE

All improvements were achieved with **$\mathcal{O}(N)$ computational
complexity**, matching standard regression losses.

---

## Key Contributions

- Novel hybrid loss function with tunable robustness
- Explicit gradient analysis explaining stability
- Improved forecasting accuracy on real public health data
- Plug-and-play compatibility with LSTM and deep learning models

---

[Access the full paper here](https://doi.org/10.1109/ACCESS.2025.3626795)

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
"A Hybrid Minkowski-Log-Cosh Loss Function for Robust LSTM-Based Time Series Forecasting,"  
*IEEE Access*, vol. 13, pp. 187307–187319, 2025,  
doi:10.1109/ACCESS.2025.3626795.

---

### Harvard
Simsoba, K.-A., Oscar, N. and Mageto, T. (2025)  
'A Hybrid Minkowski-Log-Cosh Loss Function for Robust LSTM-Based Time Series Forecasting',  
*IEEE Access*, 13, pp. 187307–187319.  
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
