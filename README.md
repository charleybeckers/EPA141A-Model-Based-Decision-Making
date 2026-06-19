# CARICOM JUSTICE Model Analysis
### EPA141A Model-Based Decision Making | COP31 Climate Negotiations | Group 9

---

## Repository structure

```
your-repo/
├── JUSTICE-main/                        ← clone the JUSTICE model here (see below)
├── caricom_justice_analysis_revised.ipynb
└── README.md

---

## Setup

**1. Clone JUSTICE**

Follow the instructions provided on Brightspace to obtain and place the `JUSTICE-main` folder.

**2. Install additional dependencies**

The following packages are required on top of the standard JUSTICE environment:

```bash
pip install ema-workbench scikit-learn seaborn
```

---

## Running the notebook

Open `caricom_justice_analysis_revised.ipynb` in Jupyter and run all cells in order. Each part is self-contained and builds on the outputs of the previous one — do not skip cells.

Expected runtime: approximately 10–20 minutes (the ensemble in Part 6 runs 576 model evaluations).

---

## Figure index

| Figure in report | Notebook section | Saved file |
|---|---|---|
| Figure A — Temperature trajectories | Part 2 | `plots_caricom/caricom_new_01_...` |
| Figure B — Emissions vs damage share | Part 3 | `plots_caricom/caricom_new_01_injustice_ratio.png` |
| Figure C — Sensitivity analysis | Part 7 | printed output |
| Figure D — Scenario discovery | Part 8 | `plots_caricom/caricom_SD_scenario_discovery.png` |
| Figure E — Robustness by ECR | Part 9 | `plots_caricom/caricom_ROB_robustness.png` |
| Figure F — Caribbean CPC trajectory | Part 5b | `plots_caricom/caricom_new_03_cpc_trajectory.png` |
| Figure G — Welfare function comparison | Part 10 | `plots_caricom/caricom_new_05_swf_regional_welfare.png` |

All figures are saved automatically to a `plots_caricom/` folder created on first run.

---

## Key modelling choices

- **Welfare function:** Sufficientarian
- **Sufficiency threshold:** 75% of Caribbean CPC along a moderate-abatement (ECR = 0.3), no-damage-scaling reference trajectory under SSP3 — see Part 0 of the notebook for full justification
- **Ensemble:** 576 runs across SSP × ECS × δ × ECR
