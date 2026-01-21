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
  <a href="{{ base_path }}/files/cv.pdf" class="btn btn--primary">
    <i class="fas fa-download"></i> Download Full CV (PDF)
  </a>
</div>

<div style="font-size: 1.06rem; line-height: 1.7;">

## Research Interests
• **Robust Machine Learning:** Methodologies and loss functions resilient to noisy data and outliers  
• **Time Series Forecasting:** Deep learning approaches for temporal prediction  
• **NLP & LLMs:** Natural Language Processing and Large Language Model applications  
• **Explainable AI (XAI):** Model interpretability and transparency  
• **Computer Vision & Speech Processing:** Advanced image and signal analysis  

## Education
• **M.Sc. in Artificial Intelligence for Science** (2025 – Present)  
  African Institute for Mathematical Sciences (AIMS), South Africa  
  *Google DeepMind Scholar*

• **Joint M.Sc. in Mathematics (Statistics Option)** (2023 – 2025)  
  Pan African University Institute for Basic Sciences, Technology and Innovation (PAUSTI), Kenya  
  *African Union Scholar*  
  *Thesis: A Hybrid Minkowski-Log-Cosh loss function for Robust LSTM-based time series forecasting*

• **B.Sc. in Mathematics, Statistics and Socio-economic Applications** (2018 – 2021)  
  Université de Kara, Togo  
  *Thesis: Evaluating the Effects of Online Learning on the Student Population of the Université de Kara During COVID-19*

## Peer-Reviewed Publications
{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

## Research Experience
• **Graduate Research Project**, PAUSTI (2024–2025)  
  • Developed a novel Hybrid Minkowski-Log-Cosh loss for robust LSTM forecasting  
  • Applied models to malaria incidence prediction using 10-year epidemiological data  

• **Undergraduate Research Project**, Université de Kara (2021–2022)  
  • Statistical analysis of online learning outcomes during the COVID-19 pandemic  

## Teaching Experience
• **Mathematics and Physics Teacher**, High Schools in Kara, Togo (2019 – 2023)  
  Delivered secondary-level instruction emphasizing conceptual understanding and problem-solving.

  **Mathematics Modules**
  • Probability and Combinatorics  
  • Set Theory and Logic  
  • Spatial Geometry (3D)  
  • Polynomial and Homographic Functions  
  • Continuity and Differentiability  
  • Arithmetic and Geometric Sequences  
  • Complex Numbers  

  **Physics Modules**
  • Kinematics and Motion under Gravity  
  • Mechanical and Electrical Oscillations  
  • Wave Phenomena and Propagation  
  • Electrostatics and RLC Circuits  
  • Thermodynamics  

• **Tutor (Volunteer)**, École Polytechnique de Lomé, Togo (2023)  
  Graduate tutoring for Master’s students in Big Data.

  **Inferential Statistics**
  • Hypothesis Testing  
  • Confidence Intervals  
  • Likelihood-Based Inference  
  • Sampling Distributions and Asymptotic Results  

  **Optimization**
  • Unconstrained and Constrained Optimization  
  • Lagrange Multipliers and KKT Conditions  
  • Gradient-Based Methods  
  • Convex Optimization  

## Technical Skills
• **Programming Languages:** Python (Advanced), R, MATLAB, SQL, C/C++  
• **AI/ML Frameworks:** TensorFlow, PyTorch, Scikit-learn, Keras  
• **Tools:** Power BI, STATA, GIS, LaTeX, GitHub, Jupyter, Overleaf  

## Awards & Honors
• **Google DeepMind Scholarship**, AIMS South Africa (2025 – 2026)  
• **African Union Scholarship**, PAUSTI Kenya (2023 – 2025)  
• **Togolese National Government Scholarship** (2015 – 2018)

</div>
