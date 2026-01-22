---
title: "A Hybrid Minkowski–Log–Cosh Loss Function for Robust LSTM-Based Time Series Forecasting"
collection: publications
category: manuscripts
permalink: /publication/2025-hybrid-minkowski-log-cosh
excerpt: >
  We propose a robust loss function
  \( \mathcal{L}_{\mathrm{MLC}}(y,\hat y)
  = \frac{1}{N}\sum_i [\log(\cosh(y_i-\hat y_i))]^p \)
  for LSTM-based time-series forecasting under noise.
date: 2025-02-15
venue: 'IEEE Access'
paperurl: 'https://doi.org/10.1109/ACCESS.2025.3626795'
citation: 'Simsoba, K.-A., Oscar, N., & Mageto, T. (2025). "A Hybrid Minkowski–Log–Cosh Loss Function for Robust LSTM-Based Time Series Forecasting." IEEE Access, 13, 187307–187319.'
mathjax: true
---

## Abstract

Robust learning is essential for time-series forecasting in real-world settings where data are noisy, irregular, or contaminated by outliers. This paper introduces a **Hybrid Minkowski–Log–Cosh (MLC) loss function**, a tunable and theoretically grounded objective designed to improve the stability and accuracy of **LSTM-based forecasting models**. The proposed approach is validated on long-horizon public health data, with a focus on malaria incidence forecasting.

---

## Loss Function Definition

Let $y_i$ and $\hat{y}_i$ denote the true and predicted values at time $i$.  
The proposed loss is defined as

\[
\mathcal{L}_{\mathrm{MLC}}(y,\hat{y})
=
\frac{1}{N}\sum_{i=1}^{N}
\left[\log\!\big(\cosh(y_i - \hat{y}_i)\big)\right]^p,
\]

where $p>0$ is a **Minkowski exponent** controlling the trade-off between robustness to outliers and error sensitivity.

**Special cases**
- $p = 1$: Log-Cosh loss  
- $p \approx 2$: MSE-like behavior  
- $p < 2$: increased robustness to outliers  

---

## Gradient Analysis

Let $\varepsilon_i = y_i - \hat{y}_i$.  
The gradient of the loss with respect to the prediction $\hat{y}_i$ is

\[
\frac{\partial \mathcal{L}_{\mathrm{MLC}}}{\partial \hat{y}_i}
=
-\,p\,\big[\log(\cosh(\varepsilon_i))\big]^{p-1}
\tanh(\varepsilon_i).
\]

This expression explains the smooth, near-quadratic behavior for small residuals
and gradient saturation for large residuals, which reduces the influence of
extreme outliers during optimization.

---

## Hessian (Curvature) Analysis

The curvature of the loss with respect to $\hat{y}_i$ is given by

\[
\frac{\partial^2 \mathcal{L}_{\mathrm{MLC}}}{\partial \hat{y}_i^2}
=
p(p-1)\big[\log(\cosh(\varepsilon_i))\big]^{p-2}\tanh^2(\varepsilon_i)
+
p\big[\log(\cosh(\varepsilon_i))\big]^{p-1}\operatorname{sech}^2(\varepsilon_i).
\]

For $p<2$, the curvature remains bounded for large residuals, providing robustness
to outliers, while $p>1$ ensures strict convexity and stable optimization.

---

## Empirical Evaluation

The loss was evaluated using **LSTM models** on **11 years (2013–2023)** of monthly
malaria incidence data.

On clean data, the MLC loss reduced **MAPE from 20.96% (MSE) to 18.23%**, while also
achieving lower MAE and RMSE. Under synthetic outlier contamination, the method
significantly reduced median absolute error and yielded approximately
**117,000 fewer mispredicted cases** compared to standard MSE training.

All improvements were achieved with **$\mathcal{O}(N)$ computational complexity**,
matching standard regression losses.

---

## Key Contributions

- **Novel hybrid loss function** with tunable robustness  
- **Theoretically grounded design** with explicit gradient and curvature analysis  
- **Improved forecasting accuracy and stability** on real public health data  
- **Plug-and-play compatibility** with LSTM and deep learning models  

---

[Access the full paper here](https://doi.org/10.1109/ACCESS.2025.3626795)

---

## How to Cite

### APA
Simsoba, K.-A., Oscar, N., & Mageto, T. (2025).  
*A Hybrid Minkowski–Log–Cosh Loss Function for Robust LSTM-Based Time Series Forecasting*.  
**IEEE Access, 13**, 187307–187319.  
https://doi.org/10.1109/ACCESS.2025.3626795

---

### IEEE
K.-A. Simsoba, N. Oscar, and T. Mageto,  
“A Hybrid Minkowski–Log–Cosh Loss Function for Robust LSTM-Based Time Series Forecasting,”  
*IEEE Access*, vol. 13, pp. 187307–187319, 2025,  
doi:10.1109/ACCESS.2025.3626795.

---

### Harvard
Simsoba, K.-A., Oscar, N. and Mageto, T. (2025)  
‘A Hybrid Minkowski–Log–Cosh Loss Function for Robust LSTM-Based Time Series Forecasting’,  
*IEEE Access*, 13, pp. 187307–187319.  
doi:10.1109/ACCESS.2025.3626795.

---

### BibTeX
```bibtex
@article{Simsoba2025MLC,
  author  = {Simsoba, Kouyakou-Abalo and Oscar, Ngesa and Mageto, Thomas},
  title   = {A Hybrid Minkowski–Log–Cosh Loss Function for Robust LSTM-Based Time Series Forecasting},
  journal = {IEEE Access},
  volume  = {13},
  pages   = {187307--187319},
  year    = {2025},
  doi     = {10.1109/ACCESS.2025.3626795}
}
