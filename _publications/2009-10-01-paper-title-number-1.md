---
title: "A Hybrid Minkowski-Log-Cosh Loss Function for Robust LSTM-Based Time Series Forecasting"
collection: publications
category: manuscripts
permalink: /publication/2025-hybrid-minkowski-log-cosh
excerpt: "This research introduces a novel hybrid loss function (MLC) designed to improve LSTM performance on noisy time-series data, specifically validated on public health datasets."
date: 2025-02-15
venue: "IEEE Access"
paperurl: "https://doi.org/10.1109/ACCESS.2025.3626795"
citation: "Simsoba, K.-A., Oscar, N., & Mageto, T. (2025). A Hybrid Minkowski-Log-Cosh Loss Function for Robust LSTM-Based Time Series Forecasting. IEEE Access, 13, 187307–187319."
mathjax: true
---

## Abstract

Robust learning is essential for time-series forecasting in real-world settings where data are noisy, irregular, or contaminated by outliers. This paper proposes a **Hybrid Minkowski–Log–Cosh (MLC) loss function**, a tunable and theoretically grounded objective designed to improve the stability and accuracy of **LSTM-based forecasting models**. The method is validated on long-horizon public health data, with a particular focus on malaria incidence forecasting.

---

## Loss Function Definition

Let $y_i$ and $\hat{y}_i$ denote the true and predicted values at time $i$.  
The proposed loss is defined as

$$
\mathcal{L}_{\mathrm{MLC}}(y,\hat{y})
=
\frac{1}{N}\sum_{i=1}^{N}
\left[\log\!\big(\cosh(y_i - \hat{y}_i)\big)\right]^p,
$$

where $p>0$ is a **Minkowski exponent** controlling the curvature of the loss and the trade-off between robustness and sensitivity.

**Special cases**
- $p = 1$: Log-Cosh loss  
- $p \approx 2$: MSE-like behavior  
- $p < 2$: increased robustness to outliers  

---

## Gradient Analysis

Let $\varepsilon_i = y_i - \hat{y}_i$ and $g_i = \log(\cosh(\varepsilon_i))$.  
The gradient with respect to the prediction $\hat{y}_i$ is

$$
\frac{\partial \mathcal{L}_{\mathrm{MLC}}}{\partial \hat{y}_i}
=
-\,p\, g_i^{\,p-1}\tanh(\varepsilon_i).
$$

**Interpretation**
- For small residuals: $\tanh(\varepsilon_i)\approx\varepsilon_i$ (smooth, MSE-like)
- For large residuals: $\tanh(\varepsilon_i)\to 1$ (gradient saturation)
- For $p<2$: extreme errors are downweighted, improving robustness

---

## Hessian and Curvature Properties

The second derivative (Hessian entry) is

$$
\frac{\partial^2 \mathcal{L}_{\mathrm{MLC}}}{\partial \hat{y}_i^2}
=
p(p-1)\, g_i^{\,p-2}\tanh^2(\varepsilon_i)
+
p\, g_i^{\,p-1}\operatorname{sech}^2(\varepsilon_i).
$$

Asymptotic behavior for large residuals:

$$
\lim_{|\varepsilon_i|\to\infty}
\frac{\partial^2 \mathcal{L}_{\mathrm{MLC}}}{\partial \hat{y}_i^2}
=
\begin{cases}
0, & 0 < p < 2, \\
2, & p = 2, \\
+\infty, & p > 2.
\end{cases}
$$

This shows that:
- **$p<2$ yields bounded curvature**, ensuring robustness to outliers
- **$p>1$ guarantees strict convexity**, enabling stable optimization
- **$p=2$ recovers MSE-like curvature**

---

## Empirical Evaluation

The loss was evaluated using **LSTM models** on **11 years (2013–2023)** of monthly malaria incidence data.

### Clean data regime (best $p=2.25$)
- **MAE:** 2,515.38  
- **MAPE:** 18.23% (↓ from 20.96% with MSE)  
- **RMSE:** 3,671.74  
- Faster convergence than MSE, MAE, and Log-Cosh  

### Noisy / outlier-contaminated regime (best $p=1.5$)
- **MAE:** 3,676.36  
- **Median AE:** 2,192.06  
- **SMAPE:** 24.63%  
- ≈ **117,000 fewer mispredicted cases** compared to MSE  

All improvements were achieved with **$\mathcal{O}(N)$ computational complexity**.

---

## Key Contributions

- **Novel loss function** with tunable robustness  
- **Explicit gradient and Hessian analysis**  
- **Improved stability and accuracy** on real public health data  
- **Plug-and-play** for LSTM and deep learning models  

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
