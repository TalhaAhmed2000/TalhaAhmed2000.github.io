---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

{% include base_path %}

Research Interests
------------------

My work sits at the intersection of **generative modelling**, **inverse problems**, and **computational imaging** — with a particular focus on making powerful models run efficiently in resource-constrained, clinically-relevant settings. I am interested in both the theoretical foundations and practical deployment of these methods.

<div class="grid" style="margin-bottom:0;">
  <section>
    <h3>Problems I Think About</h3>
    <ul>
      <li>Designing <strong>efficient generative models</strong> that avoid reliance on large pretrained backbones for downstream tasks</li>
      <li><strong>Inverse problems</strong>: image reconstruction, super-resolution, deblurring, compressed sensing</li>
      <li><strong>Model-Based Deep Learning</strong>: algorithm unrolling, unfolded optimization networks</li>
      <li><strong>Robust estimation</strong> under heavy-tailed / impulsive noise or ill-posed inverse problems</li>
      <li>Structural priors in <strong>matrix/tensor completion or generative modeling</strong> such as <strong>low-rank or sparsity</strong></li>
    </ul>
  </section>

  <section>
    <h3>Applications I Care About</h3>
    <ul>
      <li><strong>Medical Imaging</strong>: segmentation, classification, uncertainty quantification</li>
      <li><strong>Image restoration</strong>: artifact removal, denoising, inpainting</li>
      <li><strong>Generative modelling</strong> in data-scarce, unsupervised/semi-supervised settings</li>
      <li><strong>Signal processing</strong> when dealing with Principal Component Pursuit (PCP) style problems </li>
    </ul>
  </section>
</div>

<div style="text-align:center; margin: 6px 0 8px 0;">
  <img src="/files/test_3.png" alt="Research Word Cloud" style="max-width:85%; height:auto;">
</div>

Research Experience
-------------------

<div class="publication-block">
  <div class="publication-info">
    <div class="publication-title">
      Theory and Practice of Diffusion Models in Medical Imaging and Inverse Problems
    </div>
    <h3 class="conference-name">Summer 2024 – Present &nbsp;·&nbsp; ATP Lab, Electrical Engineering Department, LUMS</h3>
    <p class="author-name">with <a href="https://web.lums.edu.pk/~hmd/">Dr. Hassan Mohy-ud-Din</a></p>
    <p>
      An ongoing research assistantship where we systematically cover diffusion-based methods for inverse problems — <a href="https://arxiv.org/abs/2405.19572">BIRD</a>, <a href="https://arxiv.org/abs/2209.14687">DPS</a>, <a href="https://arxiv.org/abs/2211.10656">Blind-DPS</a>, medical imaging — <a href="https://arxiv.org/abs/2310.03559">MedSyn</a> , <a href="https://arxiv.org/abs/2406.18361">SDSeg</a>, <a href="https://arxiv.org/abs/2306.16654">SSDiffRecon</a> —, and computational imaging settings — <a href="https://arxiv.org/abs/2302.05543">ControlNet</a> , <a href="https://arxiv.org/abs/2305.07015">StableSR</a>, <a href="https://arxiv.org/abs/2308.15070">DiffBIR</a> — and more. On the practical side, this culminated in <strong>Wave-GMS</strong> (ICASSP 2026): a ~2.6M-parameter generative segmentation model trained entirely on a consumer GPU (RTX 2080 Ti, 12GB VRAM) that achieves state-of-the-art cross-domain performance.
    </p>
    <div class="links">
      <a href="https://arxiv.org/abs/2510.03216v1" class="pdf">arXiv (Wave-GMS)</a>
      <a href="https://github.com/ATPLab-LUMS/Wave-GMS" class="code">GitHub</a>
      <a href="https://drive.google.com/drive/folders/1roK1ScRDl3pC-Bq70CJ_pRBRIHqOXYjH?usp=sharing" class="pdf">Survey Draft</a>
    </div>
  </div>
</div>

<div class="publication-block">
  <div class="publication-info">
    <div class="publication-title">
      Unrolled Optimization &amp; Matrix Completion
    </div>
    <h3 class="conference-name">Spring 2023 – Spring 2024 &nbsp;·&nbsp; Senior Capstone Project, Electrical Engineering Department, LUMS</h3>
    <p class="author-name">with <a href="https://www.linkedin.com/in/muhammad-tahir-aa421590/">Dr. Muhammad Tahir</a></p>
    <p>
      Explored <strong>Model-Based Deep Learning</strong> through the lens of algorithm unrolling — bridging classical iterative solvers with trainable deep networks. Began with a reading course in High-Dimensional Data Analysis and Compressed Sensing (<a href="https://book-wright-ma.github.io/Book-WM-20210422.pdf">Wright &amp; Ma</a>), self-taught Duality Theory and the Augmented Lagrangian Method (ALM), Proximal Gradient Methods, Convex Relaxation Techniques and applied these to the Matrix Completion (MC) problem.
    </p>
    <ul>
      <li>Implemented popular deep learning algorithms from scratch (<a href="https://github.com/TalhaAhmed2000/DeepLearning">GitHub</a>) and replicated key MC baseline results (<a href="https://github.com/Talha-Nehal-Undegrad-Study/M-estimation-RMC/tree/main">GitHub</a>)</li>
      <li>Built <strong>ConvMC-Net</strong>: an unfolded ALM network for standard matrix completion (<a href="https://github.com/TalhaAhmed2000/convmc-net">GitHub</a>)</li>
      <li>Proposed <strong>ConvHuberMC-Net</strong>: an unfolded <a href="https://ieeexplore.ieee.org/document/8682657">M-estimation</a>-based network for robust MC under impulsive / heavy-tailed noise (<a href="https://github.com/Talha-Nehal-Undegrad-Study/ConvHuberMC-Net">GitHub</a>)</li>
    </ul>
    <div class="links">
      <a href="https://github.com/TalhaAhmed2000/convmc-net" class="code">ConvMC-Net</a>
      <a href="https://github.com/Talha-Nehal-Undegrad-Study/ConvHuberMC-Net" class="code">ConvHuberMC-Net</a>
    </div>
  </div>
</div>

<div class="publication-block">
  <div class="publication-info">
    <div class="publication-title">
      Mathematical Inequalities with Applications to Data Science
    </div>
    <h3 class="conference-name">Sept – Dec 2023 &nbsp;·&nbsp; Research Assistant, Electrical Engineering Department, LUMS</h3>
    <p class="author-name">with <a href="https://web.lums.edu.pk/~hmd/">Dr. Hassan Mohy-ud-Din</a></p>
    <p>
      A semester-long independent project compiling rigorous yet accessible notes on fundamental mathematical inequalities and their applications in data science and information theory. Materials were drawn from journals, conference papers, and lecture resources; each inequality is accompanied by background, a proof, key considerations, practical applications, and a Python/MATLAB demonstration.
    </p>
    <ul>
      <li>Covered inequalities from concentration inequalities and information-theoretic bounds to optimisation tools central to ML</li>
      <li>Example: <a href="https://www.dropbox.com/scl/fi/uvd6wwxslyiasaspdmngl/Jensen_s_Inequality.pdf?rlkey=csoiwfh59iyagmxy9cw66bm1v&dl=0">Jensen's Inequality</a> — proof, applications to KL divergence, convex optimisation, and Generative Adversarial Networks (GANs)</li>
      <li>Full collection available on request via <a href="mailto:hassan.mohyuddin@lums.edu.pk">Dr. Hassan</a></li>
    </ul>
  </div>
</div>

<div class="publication-block">
  <div class="publication-info">
    <div class="publication-title">
      Digital Literacy App Development
    </div>
    <h3 class="conference-name">2022 &nbsp;·&nbsp; Research Assistant, Networks Systems Group, Computer Science Department, LUMS</h3>
    <p class="author-name">with <a href="https://www.ihsanqazi.com/">Dr. Ihsan Ayub Qazi</a></p>
    <p>
      Built a digital literacy assessment app as a sequel to a <a href="https://www.sciencedirect.com/science/article/pii/S2352728523000015">published study</a> on validated digital literacy measures for low-internet-experience populations (Ali, Raza, Qazi — <em>Development Engineering</em>, 2023). The app evaluates a user's digital literacy score (0–1) from a structured questionnaire.
    </p>
    <ul>
      <li>Self-taught the <strong>Shiny</strong> framework in <strong>R</strong> and explored model deployment techniques within it</li>
      <li>Deployed a <strong>Random Forest</strong> classifier as the scoring backend, tuned on validated survey responses</li>
      <li>Designed for communities with limited prior technology exposure — simple onboarding, low-bandwidth usage</li>
    </ul>
    <div class="links">
      <a href="https://github.com/TalhaAhmed2000/Digital-Literacy-Survey-App" class="code">GitHub</a>
      <a href="https://www.sciencedirect.com/science/article/pii/S2352728523000015" class="pdf">Paper</a>
    </div>
  </div>
</div>
