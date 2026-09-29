---
layout: single
title: "About me"
permalink: /
redirect_from:
  - /about/
  - /about-me/
author_profile: true
mathjax: false
---

<p class="lede">I am <strong>Kouyakou-Abalo SIMSOBA</strong>, a Togolese AI researcher and mathematician building machine learning that can be trusted in medicine and science. I hold two Master's degrees: an M.Sc. in Artificial Intelligence for Science from AIMS South Africa and Stellenbosch University, as a <strong>Google DeepMind Scholar</strong>, and an M.Sc. in Mathematics (Statistics) from PAUSTI and JKUAT in Kenya, as an <strong>African Union Scholar</strong>. Since July 2026 I have also worked as an independent researcher, continuing my research programme on trustworthy medical artificial intelligence while I lecture discrete mathematics to future software engineers at the École Supérieure d'Audit et de Management (ESAM, the Higher School of Audit and Management) in Lomé, where I live.</p>

<p class="lede">I came to research through the classroom. I taught mathematics and physics in Togolese secondary schools for four years before turning to statistics and machine learning, and I still try to explain things plainly, whether I am writing a paper, building a model or planning a course.</p>

<div class="stat-row">
<div class="stat"><span class="n">2</span><span class="l">Master's degrees, in AI and in Statistics</span></div>
<div class="stat"><span class="n">Q1</span><span class="l">first-author paper in IEEE Access</span></div>
<div class="stat"><span class="n">ICLR 2027</span><span class="l">second paper, under review</span></div>
<div class="stat"><span class="n">84%</span><span class="l">AIMS thesis grade, with Distinction</span></div>
</div>

<div class="cv-actions"><a class="cv-btn" href="/files/cv.pdf">↓ &nbsp;Download Full CV</a></div>

<div class="section-divider"><span>Research</span></div>

<div class="kv">
<div class="kv-row"><div class="kv-label">Trustworthy medical AI</div><div class="kv-val">My M.Sc. thesis produced <strong>MultiMagNet</strong>, a four-stream ResNet-50 fusion architecture for breast cancer histopathology that reaches <strong>AUC 0.935</strong> and stays robust when magnification levels are missing. I care as much about whether a model is reliable as whether it is accurate, so I test its calibration, its uncertainty and how it behaves on unfamiliar data, and I study when it should hand a case to a human expert. I am now extending the work to multimodal fusion of images and clinical records, and to ultrasound and other imaging modalities.</div></div>
<div class="kv-row"><div class="kv-label">Robust learning &amp; forecasting</div><div class="kv-val">My first paper introduced a <strong>differentiable Minkowski-log-cosh loss</strong> for LSTM forecasting. It cuts error by 13% on 11 years of national malaria surveillance data and copes better with outliers, which are common in real health data.</div></div>
<div class="kv-row"><div class="kv-label">Computational biology</div><div class="kv-val">I model disease dynamics with compartmental and stochastic models. At the MMED clinic (ICI3D / SACEMA) my team fitted SIR, SEIR and SEIRV models to Mpox transmission in South Kivu, DRC.</div></div>
</div>

<div class="section-divider"><span>Teaching</span></div>

<p class="lede" style="font-size:1.02rem;">I began as a secondary-school teacher of mathematics and physics in Kara (2019 to 2023), tutored graduate Big Data students in statistics and convex optimization at École Polytechnique de Lomé, and now teach <em>Mathematical Tools for Software Engineering</em> (72 h, 6 ECTS) at ESAM Lomé. Each chapter starts from a real computing problem and builds the mathematics needed to solve it. <a href="/teaching/">See the syllabus →</a> · <a href="https://drive.google.com/file/d/1P10gtZbrfmMeYznHm6qZdrVbomB485W1/view?usp=sharing" target="_blank" rel="noopener">Syllabus PDF ↗</a> · <a href="https://drive.google.com/file/d/1PaXq2w45oIoPdA6XsyM6MSWV55vJnHQv/view?usp=sharing" target="_blank" rel="noopener">Course notes ↗</a></p>

<div class="section-divider"><span>Journey</span></div>

<ul class="timeline compact">
<li class="tl-item now">
<span class="tl-date">2026</span>
<div class="tl-body">Back in Lomé, I teach at ESAM and work as an independent researcher, while finishing the papers that grew out of my thesis.</div>
</li>
<li class="tl-item ">
<span class="tl-date">2025</span>
<div class="tl-body">Moved to South Africa for the M.Sc. in AI for Science at AIMS. My research turned toward medical AI.</div>
</li>
<li class="tl-item ">
<span class="tl-date">2023</span>
<div class="tl-body">Moved to Kenya for the joint M.Sc. in Mathematics (Statistics) at PAUSTI.</div>
</li>
<li class="tl-item ">
<span class="tl-date">2022</span>
<div class="tl-body">Tutored graduate statistics and optimization as a volunteer at École Polytechnique de Lomé.</div>
</li>
<li class="tl-item ">
<span class="tl-date">2019</span>
<div class="tl-body">Started teaching mathematics and physics at Kara Secondary School.</div>
</li>
<li class="tl-item ">
<span class="tl-date">2018</span>
<div class="tl-body">Began the B.Sc. at Université de Kara and graduated three years later.</div>
</li>
<li class="tl-item ">
<span class="tl-date">2015</span>
<div class="tl-body">Entered the Lycée Scientifique de Kara, the nationally selective science high school.</div>
</li>
</ul>

<div class="section-divider"><span>Research Interests</span></div>

<div class="interests">
<span class="hi">Trustworthy Medical Artificial Intelligence</span>
<span class="hi">Histopathology &amp; Ultrasound</span>
<span class="hi">Reliable &amp; Responsible AI</span>
<span>Multi-Magnification Fusion</span>
<span>Multimodal Learning</span>
<span>Uncertainty Quantification</span>
<span>Model Calibration</span>
<span>OOD Detection</span>
<span>Human-AI Deferral</span>
<span>Robust Loss Functions</span>
<span>Generative Augmentation</span>
<span>Time-Series Forecasting</span>
<span>Computational Biology</span>
<span>Epidemiological Modelling</span>
<span>Foundation Models</span>
</div>

<div class="section-divider"><span>Selected Publications</span></div>

<ul class="timeline compact">
<li class="tl-item ">
<div class="tl-head"><span class="tl-title">MultiMagNet: Multi-Magnification Fusion with Availability Masking, Magnitude Dropout, and Feature Alignment Regularisation for Robust Breast Cancer Histopathology Classification</span><span class="tl-status wip">Under review · ICLR 2027</span></div>
<div class="tl-meta"><b>Simsoba, K.-A.</b> &amp; Ezugwu, A. E.-S.</div>
<div class="tl-links"><a href="https://openreview.net/forum?id=ogfxZ1EZdq" target="_blank" rel="noopener">OpenReview ↗</a><a href="https://drive.google.com/file/d/1ye2h_KYmO1OAUOycDggAVs0YdAhbJfKy/view?usp=sharing" target="_blank" rel="noopener">Thesis PDF ↗</a><a href="https://github.com/Abalo39" target="_blank" rel="noopener">Code ↗</a></div>
</li>
<li class="tl-item ">
<div class="tl-head"><span class="tl-title">A Hybrid Minkowski-Log-Cosh Loss Function for Robust LSTM-Based Time Series Forecasting</span><span class="tl-status ok">Published · IEEE Access 2025</span></div>
<div class="tl-meta"><b>Simsoba, K.-A.</b>, Ngesa, O., &amp; Mageto, T. · vol. 13, pp. 187307 to 187319 · Q1, IF 3.9</div>
<div class="tl-links"><a href="https://doi.org/10.1109/ACCESS.2025.3626795" target="_blank" rel="noopener">DOI ↗</a><a href="https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=11220969" target="_blank" rel="noopener">PDF ↗</a><a href="https://github.com/Abalo39/Hybrid-Minkowski-Logcosh-Loss-LSTM" target="_blank" rel="noopener">Code ↗</a></div>
</li>
</ul>

<div class="section-divider"><span>Awards &amp; Honors</span></div>

<ul class="award-list">
<li><span><strong>Google DeepMind Scholar</strong>, AIMS South Africa (2025 to 2026): 1 of 40 scholars selected across Africa.</span></li>
<li><span><strong>African Union Scholar</strong>, PAUSTI (2023 to 2025): 1 of 9 national scholars in Mathematics/Statistics. <a href="https://pau-au.africa/fileadmin/user_upload/PAUSTI/pausti-coop/PAUSTI_Successful_Scholarship_Applicants__AY_2022-2023.pdf" target="_blank" rel="noopener">List ↗</a></span></li>
<li><span><strong>Ranked 1st</strong> in the graduating cohort, B.Sc. Mathematics, Statistics &amp; Applications, Université de Kara (2021).</span></li>
<li><span><strong>Togo National Scholarship</strong> for Academic Excellence, DBS-TOGO (2018 to 2021).</span></li>
<li><span><strong>National Government Scholarship</strong>, Government of Togo (2015 to 2018): top 100 secondary students nationwide.</span></li>
</ul>

<div class="section-divider"><span>News</span></div>

<ul class="timeline compact">
<li class="tl-item ">
<span class="tl-date">5 to 9 Oct 2026</span>
<div class="tl-body">Invited Speaker, African Conference for Industrial and Applied Mathematics (ACIAM), Ouagadougou, Burkina Faso. <a href="https://drive.google.com/file/d/1Y8lsSiYJ6imiWvUYQjWp2Bpvv_ULsgPG/view?usp=sharing" target="_blank" rel="noopener">Letter ↗</a></div>
</li>
<li class="tl-item ">
<span class="tl-date">Sept 2026</span>
<div class="tl-body">Joined ESAM Lomé as Lecturer: <em>Mathematical Tools for Software Engineering</em> (UE MVA003). <a href="/teaching/">Syllabus →</a></div>
</li>
<li class="tl-item ">
<span class="tl-date">Aug 2026</span>
<div class="tl-body">Attended Deep Learning Indaba 2026, Pan-Atlantic University, Lagos (2 to 7 Aug). <a href="https://drive.google.com/file/d/18ndoMZutSWAvfBRaKs8d54N_KWSQ84GA/view?usp=sharing" target="_blank" rel="noopener">Letter ↗</a></div>
</li>
<li class="tl-item ">
<span class="tl-date">Jul 2026</span>
<div class="tl-body">Completed the M.Sc. in AI for Science with Distinction, and submitted the thesis to ICLR 2027 as first author. <a href="https://drive.google.com/file/d/1ye2h_KYmO1OAUOycDggAVs0YdAhbJfKy/view?usp=sharing" target="_blank" rel="noopener">Thesis ↗</a> <a href="https://openreview.net/forum?id=ogfxZ1EZdq" target="_blank" rel="noopener">OpenReview ↗</a></div>
</li>
<li class="tl-item ">
<span class="tl-date">Jul 2026</span>
<div class="tl-body">Completed Google AI Research Foundations: LLM training and fine-tuning, LoRA, GPU-accelerated training. <a href="https://www.skills.google/public_profiles/77badf7c-2029-47f9-a95e-7ff25c3dd7cd" target="_blank" rel="noopener">Badges ↗</a></div>
</li>
<li class="tl-item ">
<span class="tl-date">Jun 2026</span>
<div class="tl-body">Attended the MMED Clinic (ICI3D / SACEMA, Stellenbosch, 15 to 26 Jun): Mpox dynamics in South Kivu, DRC. <a href="https://drive.google.com/file/d/15HbvkZ-1JzCBfbTrvKYJilkHFa5iqwfy/view?usp=sharing" target="_blank" rel="noopener">Certificate ↗</a></div>
</li>
<li class="tl-item ">
<span class="tl-date">Apr 2026</span>
<div class="tl-body">Completed <em>Decision-Aware Breast Cancer Classification</em>, mentored by Dr. Umang Bhatt. <a href="https://drive.google.com/file/d/1bb-1TDHAmVaj9zg1FgohrGYCMxGwXxnr/view?usp=sharing" target="_blank" rel="noopener">PDF ↗</a></div>
</li>
<li class="tl-item ">
<span class="tl-date">Oct 2025</span>
<div class="tl-body">First-author paper published in <a href="https://doi.org/10.1109/ACCESS.2025.3626795" target="_blank" rel="noopener">IEEE Access</a>: 13% relative MAPE improvement on 11 years of malaria surveillance data.</div>
</li>
<li class="tl-item ">
<span class="tl-date">Aug 2025</span>
<div class="tl-body">Attended Deep Learning Indaba 2025, University of Rwanda, Kigali (17 to 22 Aug). <a href="/conferences/">All conferences →</a></div>
</li>
</ul>

<div class="section-divider"><span>Toolbox</span></div>

<div class="kv">
<div class="kv-row"><div class="kv-label">Methods</div><div class="kv-val">CNNs and multimodal fusion, LSTMs and time-series forecasting, Bayesian inference, Monte Carlo methods, uncertainty quantification, generative models (diffusion, GANs, VAEs), NLP/LLMs, explainable AI, reinforcement learning.</div></div>
<div class="kv-row"><div class="kv-label">Languages &amp; frameworks</div><div class="kv-val">Python (PyTorch, TensorFlow, JAX, NumPy, Scikit-learn, Pandas), R, MATLAB, SQL, C/C++.</div></div>
<div class="kv-row"><div class="kv-label">Compute &amp; tooling</div><div class="kv-val">CUDA and GPU computing, HPC (including EuroHPC-class clusters), Docker, GCP, Git/GitHub, LaTeX, Jupyter/Colab.</div></div>
<div class="kv-row"><div class="kv-label">Spoken</div><div class="kv-val">French (native) · English (C2, fluent)</div></div>
</div>

<div class="section-divider"><span>Get in Touch</span></div>

<p class="lede" style="font-size:1.02rem;">I am looking for a <strong>fully funded Ph.D. starting in 2027</strong> in machine learning, statistics or trustworthy AI, ideally in trustworthy medical artificial intelligence. I am also open to research collaborations and to part-time visiting-lecturer (<em>vacataire</em>) teaching in statistics, probability, econometrics and machine learning. Write to me at <a href="mailto:kouyakou@aims.ac.za">kouyakou@aims.ac.za</a>.</p>
