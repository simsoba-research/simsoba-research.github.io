---
permalink: /
title: "About me!"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hello! I am **Kouyakou-Abalo SIMSOBA**, a **Google DeepMind Scholar** currently pursuing an **M.Sc. in Artificial Intelligence for Science** at **Stellenbosch University** through **AIMS South Africa**.

My research lies at the intersection of **robust machine learning**, **time-series forecasting**, and **theoretical loss-function design** for deep neural networks. I focus on developing **noise-resilient learning objectives** that improve predictive accuracy while preserving smooth optimization and interpretability in real-world data settings.

---

## Research Focus

My work addresses the following question:

> *How can we design loss functions that remain accurate, stable, and computationally efficient when data are noisy, irregular, or partially corrupted?*

To this end, I develop **hybrid and parameterized loss functions** for sequential models such as LSTMs, combining ideas from robust statistics and deep learning.

---

## Representative Contribution

In my recent work, I introduced the **Minkowski–Log–Cosh (MLC) loss**, defined as:

\[
\mathcal{L}_{\mathrm{MLC}}(y,\hat{y}) 
= \frac{1}{N}\sum_{i=1}^{N} \left[\log\!\left(\cosh(y_i - \hat{y}_i)\right)\right]^p,
\]

where \( p > 0 \) is a tunable Minkowski exponent controlling the trade-off between **robustness to outliers** and **error sensitivity**.

This formulation:
- Recovers **Log-Cosh** when \( p = 1 \)
- Behaves similarly to **MSE** when \( p \approx 2 \)
- Exhibits **gradient saturation for \( p < 2 \)**, yielding robustness to large residuals

I provided **formal proofs** of convexity, boundedness, and robustness via gradient and Hessian analysis.

---

## Quantitative Impact

Evaluated on **11 years of real malaria surveillance data**, the proposed loss achieved:

### Clean data regime
- **MAPE:** ↓ from **20.96% (MSE)** to **18.23%**
- **MAE:** ↓ by **377.47 cases**
- **RMSE:** ↓ by **258.22**
- **Training time:** faster than MSE, MAE, and Log-Cosh

This corresponds to **≈ 40,000 fewer mispredicted cases** over the forecasting horizon.

### Noisy / outlier-contaminated regime
- **MAPE:** ↓ by **3.75 percentage points**
- **Median Absolute Error:** ↓ by **843.91**
- **SMAPE:** ↓ by **1.40 percentage points**
- **≈ 117,000 fewer mispredicted cases** compared to MSE

All improvements were achieved with **\( \mathcal{O}(N) \)** computational complexity.

---

## Methodological Strengths

- Rigorous **theoretical analysis** (gradient & Hessian behavior)
- **1,584 LSTM trainings** via grid search and cross-validation
- Explicit evaluation under **both clean and noisy regimes**
- Emphasis on **real-world impact**, not only statistical metrics

---

## Background

- **M.Sc. in Mathematics** (Statistics) — *PAUSTI*, African Union Scholar  
- **B.Sc. in Mathematics & Statistics** — *Université de Kara*  

My training is rooted in **mathematical statistics**, which strongly informs my approach to machine learning model design and evaluation.

---

I am particularly interested in collaborations that **bridge mathematical theory and applied AI**, especially in **scientific forecasting, public health, and robust deep learning**.

---

**[Download my CV (PDF)](/files/cv.pdf)**
