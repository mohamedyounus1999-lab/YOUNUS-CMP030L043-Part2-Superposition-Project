# Superposition Yields Robust Neural Scaling
## Reproduction and Extension using Orthogonal Regularisation

---

## Overview

This repository contains the implementation developed for the project:

**"Superposition Yields Robust Neural Scaling: Reproduction and Extension using Orthogonal Regularisation"**

The project reproduces the core experimental framework proposed in the NeurIPS 2025 paper:

> **Superposition Yields Robust Neural Scaling**

and extends the original work by introducing **Orthogonal Regularisation** inspired by Equiangular Tight Frame (ETF) geometry to encourage more disentangled latent representations while preserving neural scaling behaviour.

The implementation is written entirely in **Python using PyTorch** and is designed to be fully reproducible.

---

## Project Objectives

The project aims to

- Reproduce the neural scaling behaviour presented in the original paper.
- Implement the baseline superposition autoencoder.
- Introduce an orthogonal regularisation strategy.
- Compare the proposed model against the baseline.
- Analyse representation efficiency, feature overlap and scaling behaviour.
- Evaluate computational efficiency and statistical significance.

---


## Features

The notebook includes

- Synthetic sparse dataset generation
- Power-law feature distribution
- Baseline superposition autoencoder
- Improved orthogonal regularised autoencoder
- Mixed Precision (AMP)
- Gradient clipping
- Cosine Annealing learning rate scheduling
- Early stopping
- Checkpointing
- Neural scaling experiments
- Strong and weak superposition experiments
- Ablation study
- Statistical significance testing
- Computational cost analysis
- Publication-quality visualisations

---

## Development Environment

The implementation was developed using

| Component | Version |
|-----------|----------|
| Python | 3.10+ |
| PyTorch | 2.x |
| CUDA | 11.x or later (optional) |
| Google Colab | Recommended |
| NumPy | Latest |
| Pandas | Latest |
| Matplotlib | Latest |
| Seaborn | Latest |
| SciPy | Latest |
| tqdm | Latest |

GPU execution is recommended but not mandatory.

---

## Installation

Clone the repository

```bash
git clone https://github.com/your-repository-name.git
```

Move into the project folder

```bash
cd your-repository-name
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

## Running the Notebook

Open

```
Superposition_Yields_Robust_Neural_Scaling.ipynb
```

using

- Google Colab (recommended)
- Jupyter Notebook
- JupyterLab

Run every cell sequentially from top to bottom.

No manual intervention is required.

---

## Experimental Workflow

```
Synthetic Feature Generation
            │
            ▼
Baseline Superposition Autoencoder
            │
            ▼
Orthogonal Regularised Autoencoder
            │
            ▼
Training
            │
            ▼
Scaling Law Experiments
            │
            ▼
Superposition Analysis
            │
            ▼
Ablation Study
            │
            ▼
Statistical Evaluation
            │
            ▼
Performance Comparison
```

---

## Hyperparameter Configuration

The notebook uses the following default configuration.

| Parameter | Value |
|-----------|---------|
| Number of Features | 256 |
| Hidden Dimensions | 16, 32, 64 |
| Learning Rate | 0.001 |
| Batch Size | 2048 |
| Maximum Epochs | 500 |
| Optimizer | AdamW |
| Scheduler | CosineAnnealingLR |
| Weight Decay | 0.0 / 0.1 |
| Orthogonal Regularisation λ | 0.05 |
| Number of Runs | 3 |
| Random Seed | 42 |

These values can be modified in the `CONFIG` dictionary within the notebook.

---

## Evaluation Metrics

The following metrics are reported:

- Validation Loss (MSE)
- Representation Fraction
- Mean Squared Overlap
- Scaling Exponent
- Training Time
- Parameter Count
- Statistical Significance (Independent t-test)

Metrics such as Accuracy, Precision, Recall, F1-score, FID and Perplexity are not used because they are not appropriate for representation learning experiments.

---

## Outputs

Running the notebook generates

- Training history
- Learning curves
- Scaling law plots
- Representation overlap plots
- Ablation study results
- Quantitative evaluation tables
- Statistical test results
- Computational cost analysis
- Final model comparison

The notebook also saves

- trained models
- figures
- evaluation tables
- experiment logs

for later analysis.

---

## Reproducibility

The implementation has been designed for reproducibility by

- fixing random seeds
- enabling deterministic PyTorch algorithms
- using reproducible dataset generation
- storing experimental configurations
- repeating experiments three times
- reporting mean and standard deviation

---

## Hardware Requirements

Minimum

- CPU
- 8 GB RAM

Recommended

- NVIDIA GPU
- CUDA support
- 12 GB RAM or greater

Google Colab GPU runtime is sufficient for reproducing all experiments.

---

## References

The implementation is based on

> *Superposition Yields Robust Neural Scaling*, NeurIPS 2025.

Additional theoretical concepts include sparse representation learning, neural scaling laws, representation superposition, and orthogonal feature regularisation.
