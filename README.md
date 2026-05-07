# Stiff ODEs: Implicit vs Explicit Euler

A numerical methods project modeling a stiff first-order chemical kinetics ODE, demonstrating why explicit Euler fails at practical step sizes and how implicit Euler remains stable. The notebook includes a closed-form solution, stability analysis, and plots comparing trajectories.

## Project Description

This project studies a stiff system derived from fast chemical decay toward a slowly varying equilibrium:

$$\frac{dC}{dt} = -k\bigl(C - C_{\text{eq}}(t)\bigr), \quad k = 10^{4}\ \text{s}^{-1}, \quad C_{\text{eq}}(t) = 1 + 0.1\sin(0.1t).$$

The fast reaction time scale ($10^{-4}$ s) and the slow equilibrium drift ($\approx 63$ s) yield a stiffness ratio of $\sim 6.3\times10^{5}$, making explicit methods impractical for stable integration over the slow dynamics.

## What the Notebook Covers

- Problem setup, parameter definitions, and analytical solution
- Stiffness analysis and explicit Euler stability limits
- Explicit Euler behavior at large, medium, and tiny time steps
- Implicit (backward) Euler formulation with Newton-Raphson updates
- Visual comparison of numerical trajectories and stability outcomes

## Requirements

- Python 3.9+
- NumPy
- Matplotlib
- Jupyter Notebook or Google Colab

## How to Run

1. Open `Stiff_ODEs_Report.ipynb` in Jupyter or Google Colab.
2. Run all cells in order to reproduce the figures and printed summaries.

## Outputs

Plots are saved to:

- `~/Downloads/` on a local machine
- `/content/` when running in Google Colab

## Repository Contents

- `Stiff_ODEs_Report.ipynb`: full report with derivations, code, and plots
