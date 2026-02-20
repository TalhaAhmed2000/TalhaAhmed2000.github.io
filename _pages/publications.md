---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

For a full list, see my [Google Scholar profile](https://scholar.google.com/citations?user=Hpt7VcMAAAAJ&hl=en).

Selected Publications
---------------------

## 2026

<div class="publication-block">
  <div class="publication-info">
    <div class="publication-title">
      Wave-GMS: Lightweight Multi-Scale Generative Model for Medical Image Segmentation
    </div>
    <img src="/files/wave-gms-diagram.png" alt="Wave-GMS Architecture Diagram" onclick="expandImage(this.src)" style="cursor:pointer; max-width:70%; display:block; margin: 12px auto;">
    <h3 class="conference-name">ICASSP 2026</h3>
    <p class="author-name"><strong>Talha Ahmed</strong>, Nehal Ahmed Shaikh, Hassan Mohy-ud-Din</p>
    <p>
      A multi-resolution generative model for medical image segmentation with only ~2.6M parameters, achieving state-of-the-art performance and strong cross-domain generalization. We combine a Haar wavelet-based encoder (ℰ<sub>wave</sub>) with a compact mask tokenizer (ℰ<sub>tiny</sub>) to eliminate reliance on large pretrained vision foundation models such as SD-VAE. A latent-alignment loss (ℒ<sub>align</sub>) ensures that LMM produces codes consistent with the decoding space of 𝒟<sub>tiny</sub>.
    </p>
    <div class="links">
      <a href="https://arxiv.org/abs/2510.03216v1" class="pdf">arXiv</a>
      <a href="https://github.com/ATPLab-LUMS/Wave-GMS" class="code">GitHub</a>
    </div>
  </div>
</div>

## In Preparation

<div class="publication-block">
  <div class="publication-info">
    <div class="publication-title">
      Unified Perspective on Diffusion Models: Theory and Practice in Medical Imaging and Inverse Problems
    </div>
    <h3 class="conference-name">Survey (In Preparation)</h3>
    <p class="author-name"><strong>Talha Ahmed</strong>, Nehal Ahmed Shaikh</p>
    <p>
      A comprehensive survey unifying theoretical perspectives on diffusion models (autoencoders, flow, energy, score-based methods) and their applications in imaging and inverse problems. Analyzes methods for segmentation, restoration, super-resolution, and generation (e.g., ControlNet, SDSeg, StableSR, ADD), highlighting fine-tuning, cross-modality learning, and latent space optimization strategies.
    </p>
    <div class="links">
      <a href="https://drive.google.com/drive/folders/1roK1ScRDl3pC-Bq70CJ_pRBRIHqOXYjH?usp=sharing" class="pdf">Draft</a>
    </div>
  </div>
</div>

<!-- Expand image box -->
<div id="imageBox" class="image-box" style="display: none;">
    <span class="close" onclick="closeImageBox()">&times;</span>
    <img class="full-image" id="expandedImage" src="" alt="Expanded Image">
</div>
<script>
    function expandImage(fullsizeSrc) {
        var imageBox = document.getElementById("imageBox");
        var expandedImg = document.getElementById("expandedImage");
        expandedImg.src = fullsizeSrc;
        imageBox.style.display = "block";
    }
    function closeImageBox() {
        var imageBox = document.getElementById("imageBox");
        imageBox.style.display = "none";
    }
</script>
