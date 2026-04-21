---
layout: page
title: "DISCO: Spatial Transcriptomics Completion"
description: Diffusion model for spatial gene expression imputation · IEEE ICIP 2025
img:
importance: 1
category: Research
related_publications: true
---

**DISCO** is a diffusion model developed at **[UC Irvine, Department of Computer Sciences](https://www.cs.uci.edu/)** for spatial transcriptomics data completion, addressing the pervasive problem of missing gene expression measurements in spatial sequencing experiments. Accepted at the **IEEE International Conference on Image Processing (ICIP) 2025**.

### Motivation

Spatial transcriptomics technologies capture gene expression while preserving tissue spatial context, but dropouts and missing values are common due to technical limitations. Standard imputation methods fail to leverage spatial dependencies between neighboring spots.

### Approach

We formulated missing-region completion as a conditional generation task and trained a diffusion model to impute missing spatial gene expression values. The model conditions on observed neighboring spots and uses denoising score matching to learn the underlying data distribution.

### Key Contributions

- Standard pipeline for spatial transcriptomics data processing, model training, missing region completion, and evaluation
- Baseline and advanced deep learning completion methods (KNN, GAN, latent space GAN) benchmarked against the diffusion approach
- Evaluation using Chamfer Distance, Earth Mover's Distance, MSE, MAE, and Cosine Similarity
- Publication-quality reproducible results

**Status:** Accepted, IEEE ICIP 2025 {% cite zhang2025disco %}
