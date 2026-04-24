# Enhancing Mutual Information Neural Estimation

This repository contains work on **Mutual Information Neural Estimation (MINE)**, with an emphasis on numerical stability, alternative objective formulations, and applications to generative modeling.

## Overview

The repository studies three closely related themes:

- **Mutual information estimation** with the original MINE objective.
- **Stabilized alternatives** based on smoother or better-behaved loss formulations.
- **GAN regularization experiments** that use MINE-inspired objectives to study training stability and mode coverage on synthetic datasets.

The implementation is notebook-first. The main deliverables are the notebooks, the written report, and the poster.

## Repository Contents

- `MINE_basic.ipynb`: core experiments on mutual information estimation and alternative loss designs.
- `MINE_GAN_circle.ipynb`: GAN experiments on a synthetic circle dataset.
- `MINE_GAN_cross.ipynb`: GAN experiments on a synthetic cross dataset.
- `EnhancedMINE.pdf`: full written report.
- `EnhancedMINE_poster.pdf`: final poster in PDF form.
- `requirements.txt`: minimal Python dependency list.
- `LICENSE`: MIT license text for the repository.

## Installation

Create a Python environment and install the listed dependencies:

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

The current `requirements.txt` includes:

- `numpy`
- `matplotlib`
- `torch`
- `jupyter`

Depending on your local notebook environment, you may choose to install additional convenience packages manually.

## Running the Notebooks

Launch Jupyter and open the notebook you want to explore:

```bash
jupyter notebook
```

Recommended order:

1. Start with `MINE_basic.ipynb` for the core estimator and loss-function comparisons.
2. Continue with `MINE_GAN_circle.ipynb` and `MINE_GAN_cross.ipynb` for the generative modeling experiments.
3. Use `EnhancedMINE.pdf` for the full narrative and `EnhancedMINE_poster.pdf` for the concise summary.

## Reproducibility Notes

- The repository is centered on notebooks rather than a packaged training framework.
- Results may vary with random seeds, notebook execution order, and local library versions.
- The report and poster include the intended interpretation of the experiments and should be read together with the notebooks.

## License

This repository is released under the **MIT License**. See `LICENSE` for details.
