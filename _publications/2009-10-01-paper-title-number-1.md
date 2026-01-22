---
title: "A Hybrid Minkowski-Log-Cosh Loss Function for Robust LSTM-Based Time Series Forecasting"
collection: publications
category: manuscripts
permalink: /publication/2025-hybrid-minkowski-log-cosh
excerpt: >
  We introduce a robust hybrid loss function for LSTM-based
  time-series forecasting, improving accuracy and stability under
  noisy and outlier-contaminated public health data.
date: 2025-02-15
venue: 'IEEE Access'
paperurl: 'https://doi.org/10.1109/ACCESS.2025.3626795'
citation: 'Simsoba, K.-A., Oscar, N., & Mageto, T. (2025). "A Hybrid Minkowski-Log-Cosh Loss Function for Robust LSTM-Based Time Series Forecasting." IEEE Access, 13, 187307–187319.'
mathjax: true
---

## Abstract

Robust learning is essential for time-series forecasting in real-world settings where data are noisy, irregular, or contaminated by outliers. This paper proposes a **hybrid loss function** designed to improve the stability and accuracy of **LSTM-based forecasting models**. The approach is validated on long-horizon public health data, with a particular focus on malaria incidence forecasting.

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

where $p>0$ is a tunable Minkowski exponent controlling the trade-off
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

This formulation yields smooth gradients for small residuals and
naturally suppresses the influence of extreme errors.

---

## Empirical Evaluation

The loss was evaluated using **LSTM models** on **11 years (2013–2023)**
of monthly malaria incidence data.

- **MAPE:** reduced from 20.96% (MSE) to 18.23%
- **MAE:** substantially lower under outlier contamination
- **Training:** faster and more stable convergence than MSE and MAE

All improvements were achieved with **$\mathcal{O}(N)$ computational
complexity**, matching standard regression losses.

---

## Key Contributions

- Robust hybrid loss function with tunable sensitivity  
- Improved forecasting accuracy under noisy conditions  
- Stable optimization for recurrent neural networks  
- Plug-and-play compatibility with deep learning frameworks  

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

### BibTeX
```bibtex
@article{Simsoba2025,
  author  = {Simsoba, Kouyakou-Abalo and Oscar, Ngesa and Mageto, Thomas},
  title   = {A Hybrid Minkowski-Log-Cosh Loss Function for Robust LSTM-Based Time Series Forecasting},
  journal = {IEEE Access},
  volume  = {13},
  pages   = {187307--187319},
  year    = {2025},
  doi     = {10.1109/ACCESS.2025.3626795}
}
