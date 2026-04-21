---
layout: page
title: Spatial Transcriptomics ML Completion Pipeline
description: Deep learning benchmark pipeline for missing region imputation · UC Irvine CS
img:
importance: 3
category: Industry
---

Machine Learning Intern at **[UC Irvine, Department of Computer Sciences](https://www.cs.uci.edu/)**, under Jing Zhang, PhD. (March 2024 – Sep 2024)

### Overview

This project contributed to the development of a benchmarking pipeline for spatial transcriptomics missing region completion — a precursor to the DISCO diffusion model project. The focus was on establishing reproducible baselines and evaluation frameworks.

### Pipeline Components

- **Data processing:** Standardized preprocessing of spatial transcriptomics datasets (normalization, quality control, masking strategies for simulating missing regions)
- **Model training:** Modular training framework supporting multiple architectures
- **Missing region completion:** Implemented and evaluated three approaches:
  - K-Nearest Neighbors (KNN) imputation
  - Generative Adversarial Network (GAN)
  - Latent Space GAN (improved spatial coherence)
- **Evaluation:** Assessed completion quality using:
  - Chamfer Distance
  - Earth Mover's Distance (EMD)
  - MSE, MAE
  - Cosine Similarity
- **Reporting:** Created reproducible, publication-quality tables in LaTeX for manuscript submission

### Impact

The pipeline and benchmarks established in this internship directly informed the design of DISCO (IEEE ICIP 2025).

**Tools:** Python, PyTorch, scikit-learn, NumPy, pandas, LaTeX
