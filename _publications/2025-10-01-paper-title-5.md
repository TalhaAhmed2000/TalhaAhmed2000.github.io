---
title: "Interpretable and Controllable Diffusion Models for Signal Processing and Semantic Correspondence"
collection: publications
time_period: Summer 2024 - Present
permalink: /publication/2024-06-01-interpretable-diffusion-models
excerpt: 'Research project focused on developing interpretable and controllable diffusion models with applications to signal processing and semantic correspondence, under the guidance of Dr. Muhammad Tahir.'
date: 2024-06-01
# venue: ''
# paperurl: ''
# citation: ''
---
Collaborating with Dr. Muhammad Tahir ([LinkedIn](https://www.linkedin.com/in/muhammad-tahir-aa421590/?originalSubdomain=pk)), this project aims to enhance the interpretability and control of diffusion models, particularly for signal processing applications where input signals deviate from conventional white noise.

- **Adapting Diffusion Models**: Our research aims to address the challenges posed by complex input signal distributions, such as Gaussian mixture model noise and structures involving low-rank and sparsity. We aim to leverage leverag score-based and flow-matching techniques to effectively adapt diffusion models to these scenarios.

- **Transporting Low-Rank Representations**: Our initial approach focuses on “transporting” low-rank representations to more familiar domains, allowing the score-based prior to adapt effectively. A related work like ‘[T-LOCO Edit](https://arxiv.org/pdf/2409.02374),’ utilizes the inherent low-rank structure of the Jacobian during the ‘Posterior Mean Prediction’ update. This technique facilitates training-free, unsupervised, interpretable, and controllable image editing but does not assume the inherent structure of the input is low-rank.

- **Evaluating Semantic Consistency**: A significant portion of our work also centers on evaluating diffusion models to ensure they generate semantically consistent and meaningful images, akin to those produced by recent advancements like Stable Diffusion 3. We will explore how to leverage this capability—either through attention maps or embeddings—extrapolating these insights within unsupervised frameworks for downstream applications, such as semantic correspondence.

- **Unified Survey**: This research complements the ongoing work with Dr. Hassan Mohy-ud-Din on *Theory and Practice of Diffusion Models in Medical Imaging and Inverse Problems*. Insights and information on both projects can be found in our comprehensive survey, accessible [here](https://drive.google.com/drive/folders/1D-vG6jOiDuBTMg74H26bAwi5SuM7A1tS?usp=sharing).


