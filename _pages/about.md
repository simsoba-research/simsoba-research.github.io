---
layout: single
title: "About me"
permalink: /
author_profile: true
mathjax: true
---

Hello! I am **Kouyakou-Abalo SIMSOBA**, a **Google DeepMind Scholar** currently pursuing an **M.Sc. in Artificial Intelligence for Science** at **Stellenbosch University** through **AIMS South Africa**.

My research lies at the intersection of **robust machine learning**, **time-series forecasting**, and **statistical learning theory**, with a focus on designing learning objectives that remain reliable under noisy, irregular, and imperfect real-world data.

---

## Research Focus

A central theme of my work is understanding how the **choice of loss function** influences the stability, accuracy, and robustness of deep neural networks, particularly recurrent architectures such as **Long Short-Term Memory (LSTM)** models.

Formally, I study learning objectives of the form

$$
\mathcal{L}(y,\hat{y})
= \frac{1}{N}\sum_{i=1}^{N} \ell\!\left(y_i - \hat{y}_i\right),
$$

and investigate principled alternatives to classical losses such as Mean Squared Error (MSE) and Mean Absolute Error (MAE), which are known to be sensitive to noise and outliers.

---

## Representative Contribution

This line of research culminated in my IEEE Access paper on **robust LSTM-based time-series forecasting**, where I introduced a novel hybrid loss function called the **Minkowski–Log–Cosh (MLC) loss**.

The MLC loss is defined as

$$
\mathcal{L}_{\mathrm{MLC}}(y,\hat{y})
= \frac{1}{N}\sum_{i=1}^{N}
\left[\log\!\big(\cosh(y_i - \hat{y}_i)\big)\right]^p,
$$

where $p>0$ is a tunable Minkowski exponent controlling the trade-off between **robustness to outliers** and **error sensitivity**.

From a theoretical perspective, I derived key properties of this loss, including strict convexity for $p>1$, bounded gradients for large residuals when $p<2$, and a smooth interpolation between MAE-like and MSE-like behavior. These properties explain why the loss remains stable during optimization while reducing the influence of extreme errors.

Empirically, when applied to **11 years of real malaria surveillance data**, this formulation improved forecasting accuracy under both clean and outlier-contaminated conditions, reducing mean absolute percentage error from **20.96% to 18.23%** on clean data and substantially lowering median absolute error under synthetic anomalies, while maintaining $\mathcal{O}(N)$ computational complexity and faster convergence compared to standard losses.

---

## Background

- **M.Sc. in Artificial Intelligence for Science**, AIMS South Africa / Stellenbosch University  
- **M.Sc. in Mathematics (Statistics)**, PAUSTI — African Union Scholar  
- **B.Sc. in Mathematics and Statistics**, Université de Kara  

My training in **mathematical statistics** strongly informs my approach to machine learning, particularly in the design and analysis of robust learning algorithms.

---

I am particularly interested in collaborations that bridge **theoretical foundations and applied AI**, especially in **scientific forecasting, public health, and robust deep learning systems**.

---

**[Download my CV (PDF)](/files/cv.pdf)**
