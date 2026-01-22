---
layout: single
title: "About me"
permalink: /
author_profile: true
mathjax: true
---

Hello! I am **Kouyakou-Abalo SIMSOBA**, a **Google DeepMind Scholar** currently pursuing an **M.Sc. in Artificial Intelligence for Science** at **Stellenbosch University** through **AIMS South Africa**.

My research lies at the intersection of **robust machine learning**, **time-series forecasting**, and **statistical learning theory**, with a focus on designing learning objectives that remain reliable under noisy and irregular real-world data.

---

## Research Focus

A central question in my work is how the choice of loss function affects the stability, accuracy, and robustness of deep neural networks, particularly recurrent architectures such as LSTMs.

Formally, I study objectives of the form

$$
\mathcal{L}(y,\hat{y})
= \frac{1}{N}\sum_{i=1}^{N} \ell\!\left(y_i - \hat{y}_i\right),
$$

and design robust alternatives to classical choices such as MSE and MAE.

---

## Representative Contribution

In recent work, I introduced the **Minkowski–Log–Cosh (MLC) loss**, defined as

$$
\mathcal{L}_{\mathrm{MLC}}(y,\hat{y})
= \frac{1}{N}\sum_{i=1}^{N}
\left[\log\!\big(\cosh(y_i - \hat{y}_i)\big)\right]^p,
$$

where $p>0$ is a tunable Minkowski exponent controlling the trade-off between **robustness to outliers** and **error sensitivity**.

Key theoretical properties include:
- strict convexity for $p>1$,
- bounded gradients and reduced influence of extreme residuals for $p<2$,
- smooth interpolation between MAE-like and MSE-like behavior.

---

## Empirical Impact

When evaluated on **11 years of real malaria surveillance data**:
- **MAPE** was reduced from **20.96% (MSE)** to **18.23%** on clean data,
- **median absolute error** decreased by over **800 cases** under synthetic outliers,
- training converged faster with overall $\mathcal{O}(N)$ computational complexity.

These improvements correspond to **tens of thousands fewer mispredicted cases** across the forecasting horizon.

---

## Background

- **M.Sc. in Artificial Intelligence for Science**, AIMS South Africa / Stellenbosch University  
- **M.Sc. in Mathematics (Statistics)**, PAUSTI — African Union Scholar  
- **B.Sc. in Mathematics and Statistics**, Université de Kara  

My training in mathematical statistics strongly informs my approach to modern machine learning.

---

I am particularly interested in collaborations that bridge **theory and application**, especially in **scientific forecasting, public health, and robust AI systems**.

---

**[Download my CV (PDF)](/files/cv.pdf)**
