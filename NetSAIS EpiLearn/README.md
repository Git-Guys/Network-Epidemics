# Network-Based SAIS Epidemic Modeling Notebook

This project contains a **PyTorch-based notebook** implementing a **Network Susceptible–Aware–Infected–Susceptible (NetSAIS)** epidemiological model.  
It demonstrates how disease spreads across **complex networks** while incorporating an **awareness state** that reduces infection risk, modeling behavioral responses such as masking or distancing.

---

## Overview

The notebook focuses on:

- **NetSAIS (Susceptible–Aware–Infected–Susceptible)**:  
  Extends the standard SIS model with an **awareness state (A)** between susceptible and infected.  
  Individuals in state **A** are less likely to become infected due to preventive behaviors, but may eventually forget and return to the susceptible state.

The model operates directly on **network structures** represented as adjacency matrices derived from NetworkX graphs, allowing realistic simulations on both small and large-scale social networks.

---

## Key Features

- **Custom graph utilities** to convert NetworkX graphs to PyTorch tensors (directed & undirected).  
- **Trainable epidemiological parameters**: infection rate (β), awareness rate (κ), infection rate for aware nodes (βₐ), recovery rate (δ), and forgetting rate (ζ).  
- **Deterministic, differentiable ODE simulation** — suitable for integration into ML pipelines.  
- **Supports large graphs** (tested with 2,500+ nodes).  
- **Visualization tools** for time-series and network snapshots.

---

## Notebook Highlights

- Simulations on multiple network topologies (e.g., Erdős–Rényi, lattice).  
- Parameter sweeps for κ and βₐ to match published SAIS model behavior.  
- Time-series plots of S, A, I fractions over simulation time.  
- Graph snapshots showing compartment states at specific timesteps.  
- Comparison to results from the original SAIS paper.

---

## Authors

- [Andrew Polyak](https://www.linkedin.com/in/andrewpolyak/)  
- [Derek Regier](https://www.linkedin.com/in/derek-regier-4a9255336/)
