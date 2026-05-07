# stiff-ODEs

This project studies a stiff ordinary differential equation from chemical kinetics and compares explicit and implicit time-integration methods.

## Project Description

The notebook models first-order chemical decay with a slowly varying equilibrium:

\[
\frac{dC}{dt} = -k\left(C - C_{\text{eq}}(t)\right), \quad
C_{\text{eq}}(t) = 1 + 0.1\sin(0.1t), \quad
k = 10^4
\]

The main goal is to show why stiffness makes explicit methods impractical and why backward Euler is effective for this type of system.

## What the Project Covers

- Problem setup and physical interpretation of the stiff system
- Stability limits for Forward Euler
- Backward Euler formulation using an implicit update
- Newton-Raphson residual and Jacobian setup
- Numerical experiments across multiple step sizes
- Error, convergence, and performance comparisons
- Final conclusions on method selection for stiff ODEs

## Main Findings

- The system is strongly stiff because fast and slow time scales are very different.
- Forward Euler becomes unstable unless the step size is extremely small.
- Backward Euler remains stable for large step sizes.
- Newton iterations converge quickly for this linear residual form.
- Implicit integration gives large computational savings for this problem.

## Repository Structure

- `Stiff_ODEs_Report.ipynb` — full report with equations, implementation, plots, and analysis

## How to Use

1. Open `Stiff_ODEs_Report.ipynb` in Jupyter Notebook or JupyterLab.
2. Run all cells to reproduce the figures and results.
3. Review sections in order from introduction to conclusions.

## Requirements

The notebook uses standard scientific Python libraries:

- `numpy`
- `matplotlib`

Install them in your Python environment before running the notebook.
