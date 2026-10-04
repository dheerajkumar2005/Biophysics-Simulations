# Computational Biophysics & Statistical Physics Simulations

[![Python 3.9+](https://img.shields.io/badge/Python-3.9%2B-blue.svg)](https://www.python.org/)
[![Physics](https://img.shields.io/badge/Physics-Statistical%20Mechanics%20%7C%20Biophysics-orange.svg)]()
[![Simulations](https://img.shields.io/badge/Methods-Monte%20Carlo%20%7C%20Langevin%20Dynamics-green.svg)]()
[![IIT Bombay](https://img.shields.io/badge/IIT%20Bombay-BB626%20Biophysics-red.svg)](https://www.iitb.ac.in/)

> **Academic Affiliation**: Course Projects for **BB 626: Biophysics & Simulations of Biological Systems**, IIT Bombay  
> **Author**: **Dheeraj Kumar Maradana** ([@dheerajkumar2005](https://github.com/dheerajkumar2005))

---

## 📌 Executive Summary

This repository contains numerical implementations, computational notebooks, and analytical reports modeling fundamental physical and biological phenomena using stochastic simulation methods.

The curriculum spans lattice spin statistics, polymer conformation thermodynamics, and stochastic differential equations governing particle diffusion in viscous cellular media.

---



---

## 🔬 Core Implementations

### 1. Metropolis Monte Carlo Ising Model (`Assignment-1/`)
* **Hamiltonian**:
  $$\mathcal{H} = -J \sum_{\langle i, j \rangle} s_i s_j - h \sum_i s_i, \quad s_i \in \{-1, +1\}$$
* **Markov Chain Dynamics**: Implements single-spin-flip Metropolis transition probabilities $P(\text{accept}) = \min(1, e^{-\beta \Delta E})$.
* **Thermodynamic Observables**: Tracks energy relaxation trajectories, spontaneous magnetization, and hysteresis loops across coupling ratios $J/k_B T$.

### 2. Polymer Chain Scaling & Conformations (`Assignment-2/`)
* Simulates polymer chain expansion on discrete lattices comparing freely jointed chains against excluded volume interactions.
* Computes scaling relations between contour length $N$ and root-mean-square end-to-end distance $\sqrt{\langle R^2 \rangle} \propto N^\nu$.

### 3. Brownian Motion & Langevin Dynamics (`Assignment-3/`)
* **Stochastic Integration**: Solves the Langevin equation with Gaussian white-noise thermal force $\langle \xi(t) \xi(t') \rangle = 2 \gamma k_B T \, \delta(t - t')$.
* **Fluctuation-Dissipation**: Validates Einstein's diffusion relation $D = k_B T / \gamma$ across simulated ensembles.
* **Velocity Autocorrelation (VACF)**: Demonstrates exponential decay of velocity correlations under hydrodynamic drag.

---

## 📁 Repository Structure

```
├── Assignment-1/               # 1D/2D Ising model Monte Carlo simulation notebooks and reports
│   ├── assignment1.ipynb       # Metropolis simulation notebook
│   └── assignment1.pdf         # Complete report with energy/magnetization plots
├── Assignment-2/               # Polymer physics, chain conformation, and scaling laws
│   ├── assignment2.ipynb       # Polymer walk simulation notebook
│   └── assignment2.pdf         # Analytical report
└── Assignment-3/               # Brownian motion and Langevin equation integration
    ├── Brownian.ipynb          # Langevin dynamics simulation
    └── Assignement_3.pdf       # Technical report on diffusion and MSD regimes
```

---

## 🚀 Getting Started

```bash
git clone https://github.com/dheerajkumar2005/BB626-Biophysics-Simulations.git
cd BB626-Biophysics-Simulations

pip install numpy scipy matplotlib seaborn jupyter

jupyter notebook Assignment-1/assignment1.ipynb
```
