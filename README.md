# Digital Health Design for Systemic Leverage: 60-Month System Dynamics Simulator

[![Live Simulator](https://img.shields.io/badge/Live_SD_Simulator-GitHub_Pages-008080?style=for-the-badge)](https://japarravalencia.github.io/dh-leverage-points/)
[![Zenodo DOI](https://img.shields.io/badge/Zenodo_DOI-10.5281%2Fzenodo.XXXXXXX-0f2648?style=for-the-badge)](https://doi.org/10.5281/zenodo.XXXXXXX)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg?style=for-the-badge)](https://creativecommons.org/licenses/by/4.0/)

Open Science replication package and browser-native interactive simulator accompanying the research manuscript submitted to *Simulation Modelling Practice and Theory* (Elsevier):

> **Parra Valencia, J. A., Ospina, A., Ospina, D., Suárez, F., Solano, A., Peláez, C., & Parra, H. (2026).** *Digital Health Design for Systemic Leverage: A System Dynamics Simulation and Global Sensitivity Assessment of EHR Interoperability, Value-Based Care, and the Goodhart Trap in Chronic Care Ecosystems.*

## Quick Links
- **Interactive Web Flight Simulator (GitHub Pages):** https://japarravalencia.github.io/dh-leverage-points/
- **Permanent Archive (Zenodo):** https://doi.org/10.5281/zenodo.XXXXXXX

## Package Contents
- `index.html` — Standalone browser-based 60-month System Dynamics simulator (`dt = 0.25` months) with live Meadows leverage controls (`LP6` EHR Interoperability, `LP5` Value-Based Reimbursement, `LP2` KPI Mental Model), health-equity context strata, active fatigue relief sensitivity, 6 published presets, and CSV export.
- `sfd dh leverage points 5 julio 2026.stmx` — Native OASIS XMILE 1.0 Stock-and-Flow model (4 stocks, 8 flows, 6 auxiliaries, 17 parameters).
- `CLD DH leveravege points 5 julio 2026.stmx` — Companion Causal Loop Diagram in OASIS XMILE format.
- `experimentos_dh_leverage_sobol.py` — Deterministic Python verification suite reproducing 9 scenarios, Stella–Python numerical concordance (`max abs diff <= 0.0049`), 3-step Richardson convergence (`dt = 0.25 / 0.125 / 0.0625` m) and RK4 cross-check, Barlas unclamped boundary/flow conservation (`8.53e-14`), exact bifurcation threshold (`EHR* = 0.72`), equity-stratified sensitivity, and Saltelli–Sobol global sensitivity with second-order interaction indices (`S_ij`).
- `*.csv` & `corridas_csv/` — Precomputed verified trajectories, concordance tables, bifurcation grid, and Sobol ensembles.

## Ethics & Data Statement
This package contains exclusively synthetic mechanistic simulation models and outputs. Zero individual human-subject records or personally identifiable data are used or archived.
