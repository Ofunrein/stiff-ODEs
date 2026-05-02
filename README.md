# stiff-ODEs

This repository contains a complete stiff-ODE numerical methods project focused on modeling and solving a stiff first-order system with implicit methods.

## Project Scope

- Problem type: stiff ordinary differential equations
- Core objective: show stiffness behavior and compare stable/unstable numerical integration behavior
- Method focus: explicit Euler (failure regime) and implicit/backward Euler (stable regime)
- Deliverable style: technical report with equations, implementation, plots, and interpretation

## Files

- `Stiff_ODEs_Report.ipynb`: primary source notebook with code and narrative

## Contents Overview

The report/notebook covers:
- system definition and parameter setup for a stiff ODE
- numerical stability motivation for time-step selection
- implementation of explicit and implicit update schemes
- equation setup for implicit residual/Jacobian terms
- Newton-style solve flow (where applicable)
- visual comparison of numerical trajectories
- concise interpretation of model and method behavior

## How To Use This Repo

1. Open `Stiff_ODEs_Report.ipynb` to inspect code cells and rerun computations.
