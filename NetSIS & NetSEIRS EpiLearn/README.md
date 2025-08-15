# Network-Based Epidemic Modeling Notebook

This project contains a **PyTorch-based notebook** implementing two network-based epidemiological models: **NetSIS** and **NetSEIRS**. The notebook demonstrates how disease spreads across networks and how network structure influences epidemic dynamics.

---

## Overview

The notebook focuses on:

- **NetSIS (Susceptible–Infected–Susceptible)**:  
  Simulates diseases without lasting immunity. Nodes can be reinfected over time.

- **NetSEIRS (Susceptible–Exposed–Infected–Recovered–Susceptible)**:  
  Simulates diseases with an incubation period, recovery, and temporary immunity.

Both models operate directly on network data, represented as adjacency matrices derived from NetworkX graphs. This allows realistic simulations on small social networks (e.g., Karate Club) or subsets of larger networks (e.g., Facebook connections).

---

## Key Features

- Custom graph utilities to convert NetworkX graphs to PyTorch tensors.  
- Trainable epidemiological parameters (infection, recovery, incubation, immunity loss rates).  
- Time-series simulations to track node-level infection dynamics.  
- Visualizations of both network state and compartment-level dynamics over time.

---

## Notebook Highlights

- Demonstrates forward simulation of SIS and SEIRS models on small networks.  
- Explores how network structure (directed vs. undirected) affects spread.  
- Provides plots of node-level states and overall compartment fractions over time.  
- Useful as a learning tool for graph-based epidemiology and PyTorch modeling.

---

## Authors

- [Andrew Polyak](https://www.linkedin.com/in/andrewpolyak/)  
- [Derek Regier](https://www.linkedin.com/in/derek-regier-4a9255336/)

