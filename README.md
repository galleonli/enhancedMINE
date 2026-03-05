## Enhancing Mutual Information Neural Estimation

This repository contains the code and materials for an extended study of Mutual Information Neural Estimation (MINE), with both theoretical analysis and practical applications to generative models.

The project was originally developed as a final project for the course **Fundamentals of Information Theory (EE142), 2024 Fall, ShanghaiTech University** and has been adapted here for public release.

### Overview

- **Robust mutual information estimation**: Investigates numerical challenges arising from logarithmic and exponential terms in the original MINE objective and proposes alternative loss formulations.
- **Stabilized training objectives**: Explores variants based on Softplus, Log-Sum-Exp, and regularized losses to improve stability and reduce gradient pathologies.
- **Applications to GANs**: Uses MINE-based regularization to improve mode coverage in Generative Adversarial Networks, studying how mutual-information-based terms affect stability and mode collapse.

### Repository structure

- `MINE_basic.ipynb`  
  Core experiments on mutual information estimation, including alternative loss functions and numerical behavior.

- `MINE_GAN_circle.ipynb`  
  Experiments applying MINE-based regularization to GANs on a synthetic "circle" dataset to study mode coverage and training stability.

- `MINE_GAN_cross.ipynb`  
  Similar experiments on a "cross" dataset, comparing different mutual-information-based regularizers and their effect on generated samples.

- `poster/`  
  LaTeX source, figures, and assets for the project poster that summarizes the main ideas, methods, and results.

- `EnhancedMINE.pdf`  
  Written project report with detailed derivations, methodology, and experimental results.

- `EnhancedMINE_poster.pdf`  
  A compiled PDF version of the project poster.

### Getting started

1. **Clone the repository**

```bash
git clone https://github.com/<your-username>/enhancedMINE.git
cd enhancedMINE
```

2. **Set up a Python environment**

Create and activate a virtual environment (optional but recommended), then install the required packages (e.g. `torch`, `numpy`, `matplotlib`, `tqdm`, `jupyter`):

```bash
pip install -r requirements.txt
```

or manually install the dependencies used in the notebooks.

3. **Launch Jupyter**

```bash
jupyter notebook
```

Open any of the notebooks (e.g. `MINE_basic.ipynb`) to explore and run the experiments.

### Notes on source material

The first part of both the written report and the poster summarizes and excerpts key definitions, formulations, and experimental descriptions from the original MINE paper.  
The main contributions of this project are the extended analysis of numerical issues, the design and comparison of alternative loss functions, and the new experiments on GAN mode coverage.

### Reproducing experiments

- Start with `MINE_basic.ipynb` to understand and reproduce the core mutual information estimation experiments and loss-function variants.
- Then run `MINE_GAN_circle.ipynb` and `MINE_GAN_cross.ipynb` to reproduce the GAN experiments on synthetic datasets and compare different regularization strategies.
- For a high-level summary, consult the poster in `poster/` and the poster snapshots above.

### How to cite / acknowledge

If you use this repository or build on its ideas, please acknowledge:

> Enhancing Mutual Information Neural Estimation: Theoretical Insights and Practical Applications,  
> Final project for Fundamentals of Information Theory (EE142), ShanghaiTech University, 2024 Fall.

### License

This project is released under the **MIT License**.  
See the `LICENSE` file for full terms.
