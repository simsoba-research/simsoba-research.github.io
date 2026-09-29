---
layout: single
title: ""
permalink: /
redirect_from:
  - /about/
  - /about-me/
author_profile: true
mathjax: false
---

<p class="lede">I am <strong>Kouyakou-Abalo SIMSOBA</strong>, an AI researcher and mathematician from Togo. I hold two Master's degrees — an M.Sc. in Artificial Intelligence for Science from AIMS South Africa and Stellenbosch University, and an M.Sc. in Mathematics (Statistics) from PAUSTI and JKUAT in Kenya. I now live in Lomé, where I work on trustworthy medical AI and lecture at ESAM.</p>

<p class="lede">My current focus is on making deep learning models reliable in clinical settings — not just accurate, but calibrated, well-understood, and honest about what they don't know. I am looking for a <strong>fully funded Ph.D. position starting in 2027</strong>.</p>

<div class="stat-row">
<div class="stat"><span class="n">2</span><span class="l">Master's degrees, in AI and in Statistics</span></div>
<div class="stat"><span class="n">Q1</span><span class="l">first-author paper in IEEE Access</span></div>
<div class="stat"><span class="n">Distinction</span><span class="l">AIMS M.Sc. thesis</span></div>
<div class="stat"><span class="n">1st</span><span class="l">ranked in B.Sc. cohort, Université de Kara</span></div>
</div>

<div class="cv-actions"><a class="cv-btn" href="/files/cv.pdf">↓ &nbsp;Download CV</a></div>

<div class="section-divider"><span>Research</span></div>

<div class="kv">
<div class="kv-row"><div class="kv-label">Medical imaging</div><div class="kv-val">Breast cancer histopathology is hard partly because the same tissue looks different at different magnifications — and most systems pick one. My M.Sc. thesis built <strong>MultiMagNet</strong>, a four-stream ResNet-50 that fuses all four BreakHis magnification levels simultaneously, reaching AUC 0.935 while staying robust when magnifications are missing at inference. I evaluated calibration, uncertainty, and out-of-distribution behaviour alongside raw accuracy. I'm now extending it to fuse imaging with clinical records. The paper is under review at ICLR 2027. <a href="https://openreview.net/forum?id=ogfxZ1EZdq" target="_blank" rel="noopener">OpenReview ↗</a></div></div>
<div class="kv-row"><div class="kv-label">Robust forecasting</div><div class="kv-val">Health surveillance data is messy — outliers are common, and standard losses like MSE punish them disproportionately. My first paper designed a differentiable loss combining Minkowski and log-cosh terms to handle this better. On 11 years of Kenyan malaria surveillance data it reduced forecasting error by 13% relative to MSE. Published in <em>IEEE Access</em> (Q1, IF 3.9). <a href="https://doi.org/10.1109/ACCESS.2025.3626795" target="_blank" rel="noopener">DOI ↗</a></div></div>
<div class="kv-row"><div class="kv-label">Epidemiological modelling</div><div class="kv-val">At the MMED clinic (ICI3D / SACEMA, Stellenbosch) I worked on SIR, SEIR, and stochastic SEIRV models of Mpox transmission in South Kivu, DRC — fitting parameters from real surveillance data and estimating intervention effects.</div></div>
</div>

<div class="section-divider"><span>Journey</span></div>

<ul class="timeline compact">
<li class="tl-item now">
<span class="tl-date">2026</span>
<div class="tl-body">Completed the AIMS M.Sc. with Distinction. Submitted MultiMagNet to ICLR 2027. Joined ESAM Lomé as lecturer. Invited speaker at ACIAM, Ouagadougou (Oct).</div>
</li>
<li class="tl-item ">
<span class="tl-date">2025</span>
<div class="tl-body">Google DeepMind Scholar at AIMS South Africa. First-author paper published in <em>IEEE Access</em>.</div>
</li>
<li class="tl-item ">
<span class="tl-date">2023</span>
<div class="tl-body">African Union Scholar at PAUSTI, Kenya — one of 9 national scholars in Mathematics/Statistics. Began the M.Sc. in Mathematics (Statistics).</div>
</li>
<li class="tl-item ">
<span class="tl-date">2022</span>
<div class="tl-body">Volunteer graduate tutor in statistics and optimization, École Polytechnique de Lomé.</div>
</li>
<li class="tl-item ">
<span class="tl-date">2019</span>
<div class="tl-body">Mathematics and physics teacher, Kara Secondary School, Togo.</div>
</li>
<li class="tl-item ">
<span class="tl-date">2018</span>
<div class="tl-body">B.Sc. in Mathematics, Statistics and Socio-Economic Applications, Université de Kara — <em>Mention Bien</em>, ranked 1st in the cohort.</div>
</li>
<li class="tl-item ">
<span class="tl-date">2015</span>
<div class="tl-body">Lycée Scientifique de Kara, on a National Government Scholarship for the top 100 secondary students in Togo.</div>
</li>
</ul>

<div class="section-divider"><span>Research Interests</span></div>

<div class="interests">
<span class="hi">Trustworthy Medical AI</span>
<span class="hi">Histopathology &amp; Medical Imaging</span>
<span class="hi">Uncertainty Quantification</span>
<span>Model Calibration</span>
<span>OOD Detection</span>
<span>Human-AI Deferral</span>
<span>Multi-Magnification Fusion</span>
<span>Robust Loss Functions</span>
<span>Time-Series Forecasting</span>
<span>Epidemiological Modelling</span>
</div>

<div class="section-divider"><span>Selected Publications</span></div>

<ul class="timeline compact">
<li class="tl-item ">
<div class="tl-head"><span class="tl-title">MultiMagNet: Multi-Magnification Fusion with Availability Masking, Magnitude Dropout, and Feature Alignment Regularisation for Robust Breast Cancer Histopathology Classification</span><span class="tl-status wip">Under review · ICLR 2027</span></div>
<div class="tl-meta"><b>Simsoba, K.-A.</b> &amp; Ezugwu, A. E.-S.</div>
<div class="tl-links"><a href="https://openreview.net/forum?id=ogfxZ1EZdq" target="_blank" rel="noopener">OpenReview ↗</a><a href="https://drive.google.com/file/d/1ye2h_KYmO1OAUOycDggAVs0YdAhbJfKy/view?usp=sharing" target="_blank" rel="noopener">Thesis PDF ↗</a><a href="https://github.com/Abalo39" target="_blank" rel="noopener">Code ↗</a></div>
</li>
<li class="tl-item ">
<div class="tl-head"><span class="tl-title">A Hybrid Minkowski–Log-Cosh Loss Function for Robust LSTM-Based Time Series Forecasting</span><span class="tl-status ok">Published · IEEE Access 2025</span></div>
<div class="tl-meta"><b>Simsoba, K.-A.</b>, Ngesa, O., &amp; Mageto, T. · vol. 13, pp. 187307–187319 · Q1, IF 3.9</div>
<div class="tl-links"><a href="https://doi.org/10.1109/ACCESS.2025.3626795" target="_blank" rel="noopener">DOI ↗</a><a href="https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=11220969" target="_blank" rel="noopener">PDF ↗</a><a href="https://github.com/Abalo39/Hybrid-Minkowski-Logcosh-Loss-LSTM" target="_blank" rel="noopener">Code ↗</a></div>
</li>
</ul>

<div class="section-divider"><span>Awards</span></div>

<ul class="award-list">
<li><span><strong>Google DeepMind Scholar</strong>, AIMS South Africa (2025–2026) — 1 of 40 across Africa.</span></li>
<li><span><strong>African Union Scholar</strong>, PAUSTI (2023–2025) — 1 of 9 national scholars in Mathematics/Statistics. <a href="https://pau-au.africa/fileadmin/user_upload/PAUSTI/pausti-coop/PAUSTI_Successful_Scholarship_Applicants__AY_2022-2023.pdf" target="_blank" rel="noopener">List ↗</a></span></li>
<li><span>Ranked <strong>1st</strong> in the graduating cohort, B.Sc. Mathematics, Université de Kara (2021).</span></li>
<li><span>Togo National Scholarship for Academic Excellence, DBS-TOGO (2018–2021).</span></li>
<li><span>National Government Scholarship, Government of Togo (2015–2018) — top 100 students nationwide.</span></li>
</ul>

<div class="section-divider"><span>News</span></div>

<ul class="timeline compact">
<li class="tl-item ">
<span class="tl-date">Oct 2026</span>
<div class="tl-body">Invited speaker at <strong>ACIAM</strong>, Ouagadougou, Burkina Faso. <a href="https://drive.google.com/file/d/1Y8lsSiYJ6imiWvUYQjWp2Bpvv_ULsgPG/view?usp=sharing" target="_blank" rel="noopener">Letter ↗</a></div>
</li>
<li class="tl-item ">
<span class="tl-date">Sept 2026</span>
<div class="tl-body">Joined ESAM Lomé as Lecturer — <em>Mathematical Tools for Software Engineering</em>.</div>
</li>
<li class="tl-item ">
<span class="tl-date">Aug 2026</span>
<div class="tl-body"><strong>Deep Learning Indaba 2026</strong>, Pan-Atlantic University, Lagos. <a href="https://drive.google.com/file/d/18ndoMZutSWAvfBRaKs8d54N_KWSQ84GA/view?usp=sharing" target="_blank" rel="noopener">Letter ↗</a></div>
</li>
<li class="tl-item ">
<span class="tl-date">Jul 2026</span>
<div class="tl-body">Completed the M.Sc. with Distinction. MultiMagNet submitted to ICLR 2027. <a href="https://openreview.net/forum?id=ogfxZ1EZdq" target="_blank" rel="noopener">OpenReview ↗</a></div>
</li>
<li class="tl-item ">
<span class="tl-date">Jun 2026</span>
<div class="tl-body"><strong>MMED Clinic</strong>, ICI3D / SACEMA, Stellenbosch — Mpox dynamics modelling. <a href="https://drive.google.com/file/d/15HbvkZ-1JzCBfbTrvKYJilkHFa5iqwfy/view?usp=sharing" target="_blank" rel="noopener">Certificate ↗</a></div>
</li>
<li class="tl-item ">
<span class="tl-date">Oct 2025</span>
<div class="tl-body">First-author paper published in <a href="https://doi.org/10.1109/ACCESS.2025.3626795" target="_blank" rel="noopener">IEEE Access</a>.</div>
</li>
<li class="tl-item ">
<span class="tl-date">Aug 2025</span>
<div class="tl-body"><strong>Deep Learning Indaba 2025</strong>, University of Rwanda, Kigali. <a href="/conferences/">All conferences →</a></div>
</li>
</ul>

<div class="section-divider"><span>Toolbox</span></div>

<div class="kv">
<div class="kv-row"><div class="kv-label">Core skills</div><div class="kv-val">CNNs and multimodal fusion, LSTMs and time-series forecasting, Bayesian inference, Monte Carlo methods, calibration and uncertainty quantification, OOD detection, differentiable loss design.</div></div>
<div class="kv-row"><div class="kv-label">Languages &amp; frameworks</div><div class="kv-val">Python (PyTorch, TensorFlow, JAX, NumPy, Scikit-learn, Pandas), R, MATLAB, SQL, C/C++.</div></div>
<div class="kv-row"><div class="kv-label">Compute &amp; tooling</div><div class="kv-val">CUDA, GPU computing, HPC (EuroHPC-class clusters), Docker, Git/GitHub, LaTeX, Jupyter/Colab.</div></div>
<div class="kv-row"><div class="kv-label">Languages</div><div class="kv-val">French (native) · English (C2)</div></div>
</div>

<div class="section-divider"><span>Contact</span></div>

<p class="lede" style="font-size:1.02rem;">Open to Ph.D. opportunities, research collaborations, and part-time teaching. Write to me at <a href="mailto:kouyakou@aims.ac.za">kouyakou@aims.ac.za</a>.</p>
