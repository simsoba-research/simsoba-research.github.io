---
layout: single
title: "About me"
permalink: /
author_profile: true
mathjax: true
---

Hello! I am **Kouyakou-Abalo SIMSOBA**, a **Google DeepMind Scholar** pursuing an **M.Sc. in Artificial Intelligence for Science** at **Stellenbosch University** through **AIMS South Africa**.

My research focuses on **robust machine learning** and **time-series forecasting**, with an emphasis on designing learning objectives that remain stable and accurate under noisy and irregular real-world data.

---

## Research Focus

A central question in my work is how the **choice of loss function** affects the optimization and robustness of deep neural networks, particularly **LSTM-based** models.

I study learning objectives of the form

$$
\mathcal{L}(y,\hat{y})
= \frac{1}{N}\sum_{i=1}^{N} \ell\!\left(y_i - \hat{y}_i\right),
$$

and develop principled alternatives to classical losses such as MSE and MAE.

---

## Representative Contribution

This work culminated in my **IEEE Access** paper on robust LSTM-based time-series forecasting, where I introduced the **Minkowski–Log–Cosh (MLC) loss**:

$$
\mathcal{L}_{\mathrm{MLC}}(y,\hat{y})
= \frac{1}{N}\sum_{i=1}^{N}
\left[\log\!\big(\cosh(y_i - \hat{y}_i)\big)\right]^p,
$$

with $p>0$ controlling the trade-off between **robustness to outliers** and **error sensitivity**.

To understand its behavior, I performed a **gradient and Hessian analysis**, showing that:
- for $p<2$, gradients saturate for large residuals, reducing the influence of outliers;
- for $p>1$, the loss is strictly convex, ensuring stable optimization;
- the curvature interpolates smoothly between MAE-like and MSE-like regimes.

Empirical evaluation on **11 years of malaria surveillance data** confirmed these theoretical insights, yielding improved accuracy and faster convergence under both clean and outlier-contaminated conditions.

---

## Background

- **M.Sc. in Artificial Intelligence for Science**, AIMS South Africa / Stellenbosch University  
- **M.Sc. in Mathematics (Statistics)**, PAUSTI — African Union Scholar  
- **B.Sc. in Mathematics and Statistics**, Université de Kara  

My background in **mathematical statistics** strongly informs my approach to robust learning and model analysis.

---

I am interested in collaborations at the intersection of **theory and applied AI**, particularly in **scientific forecasting, public health, and robust deep learning**.

---

**[Download my CV (PDF)](/files/cv.pdf)**
