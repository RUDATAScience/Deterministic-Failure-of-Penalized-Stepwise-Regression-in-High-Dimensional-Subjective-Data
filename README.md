# The Illusion of Parsimony: Deterministic Failure of Penalized Stepwise Regression in High-Dimensional Subjective Data

[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Paper: MDPI Computation](https://img.shields.io/badge/Paper-Submitted-success.svg)](#)

## Overview
This repository contains the official Monte Carlo simulation code, datasets, and high-resolution figures for the research paper: **"The Illusion of Parsimony: Mathematical Invalidation of AIC and BIC Penalization in Multidimensional Big Data"**. 

The study systematically deconstructs the mathematical and topological failure mechanisms of maximum likelihood estimation and penalized stepwise variable selection (AIC/BIC) when applied to bounded, sparse, and cognitively skewed subjective data (e.g., Likert scales, behavioral logs).

## Core Framework & Hypotheses
The simulations evaluate likelihood divergence, penalization limits, and parameter convergence across logarithmic scaling intervals (from $N=1,000$ to $N=10,000,000$) through a six-stage framework:

*   **H1 (Geometric Constraints):** Baseline likelihood bounds in independent discrete geometries.
*   **H2 (Thermodynamic Cognitive Noise):** Parameter variance inflation via distributional skewness.
*   **H3 (Micro-Cell Combinatorial Divergence):** Localized complete separation and macroscopic log-likelihood explosion triggered by interaction terms.
*   **H4 (Big Data Penalty Invalidation):** The $\mathcal{O}(N)$ likelihood inflation overriding the logarithmic $\mathcal{O}(\ln N)$ BIC penalty in massive datasets.
*   **H5 (Automated P-Hacking):** Deterministic failure of stepwise selection (FWER = 1.000).
*   **H6 (Coefficient Contamination):** Absolute algebraic determinism where the estimated coefficient magnitude is a strict inverse projection of distributional rarity ($\vert{}\hat{\beta}\vert{} \propto 1/p$).
