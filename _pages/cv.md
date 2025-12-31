---
layout: archive
title: "Curriculum Vitae"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<div class="cv-download-links">
  <a href="{{ base_path }}/files/cv.pdf" class="btn btn--primary"><i class="fas fa-download"></i> Download Full CV (PDF)</a>
</div>

## Research Interests
* **Robust Machine Learning:** Developing methodologies and loss functions resilient to noisy data and outliers.
* **Time Series Forecasting:** Deep learning approaches for temporal data analysis and prediction.
* **NLP & LLMs:** Natural Language Processing and Large Language Model applications.
* **Explainable AI (XAI):** Enhancing model interpretability and transparency.
* **Computer Vision & Speech Processing:** Advanced signal and image analysis techniques.

## Education
* **M.Sc. in Artificial Intelligence for Science**, African Institute for Mathematical Sciences (AIMS), South Africa | 2023 – 2025
  * **Google DeepMind Scholar**
* **Joint M.Sc. in Mathematics (Statistics Option)**, Pan African University Institute for Basic Sciences, Technology and Innovation (PAUSTI), Kenya | 2021 – 2023
  * *Thesis: A Hybrid Minkowski-Log-Cosh loss function for Robust LSTM-based time series forecasting*
  * *African Union Scholar*
* **B.Sc. in Mathematics, Statistics and Socio-economic Applications**, Université de Kara, Togo | 2018 – 2021
  * *Thesis: Evaluating the Effects of Online Learning on the Student Population of the Université de Kara During the COVID-19 Pandemic*

## Peer-Reviewed Publications

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

## Research Experience
* **Graduate Research Project**, Pan African University Institute for Basic Sciences, Technology and Innovation (PAUSTI) | 2024–2025
  * Developed a novel **hybrid Minkowski-Log-Cosh loss function** to enhance LSTM robustness against outliers in time series forecasting.
  * Applied LSTM models to predict malaria case incidence using 10 years of epidemiological data (2013-2023), demonstrating improved accuracy in noisy public health datasets.

* **Undergraduate Research Project**, Université de Kara | 2021–2022
  * Designed **Artificial Neural Network (ANN) models** for agricultural yield prediction, integrating climate, soil, and environmental variables.
  * Conducted feature sensitivity analysis to identify key predictive factors for crop productivity optimization.

## Teaching Experience
* **Mathematics and Physics Teacher**, High Schools, Kara, Togo | 2019–2023
  * Delivered comprehensive high school curriculum in **Physics** (Kinematics, Thermodynamics, Electricity) and **Mathematics** (Probability, Analysis, Geometry).
  * Developed interactive lesson plans and assessment tools to enhance student engagement and understanding of complex scientific concepts.

* **Tutor (Volunteer)**, École Polytechnique de Lomé, Togo | 2023
  * Instructed Master's students in the Big Data program on **Inferential Statistics** (hypothesis testing, confidence intervals) and **Optimization** techniques (KKT Conditions, Gradient-based methods).
  * Provided academic support and developed specialized course materials for advanced analytical coursework.

## Technical Skills
* **Programming Languages:** Python (Advanced), R, MATLAB, SQL, C/C++
* **AI/ML Frameworks & Libraries:** TensorFlow, PyTorch, Scikit-learn, Keras, Pandas, NumPy
* **Data Analysis & Visualization:** Power BI, STATA, SPSS, GIS (Geographic Information Systems)
* **Research & Development Tools:** LaTeX, GitHub, Jupyter Notebooks, Google Colab, Overleaf
* **Specialized Domains:** Time Series Analysis, Natural Language Processing, Computer Vision, Explainable AI

## Awards & Honors
* **Google DeepMind Scholarship**, African Institute for Mathematical Sciences (AIMS) | 2025–2026
* **African Union Scholarship**, Pan African University Institute for Basic Sciences, Technology and Innovation (PAUSTI) | 2023–2025
* **Togolese National Government Scholarship**, Government of Togo | 2015–2018
