# CARICOM JUSTICE Model Analysis
### EPA141A Model-Based Decision Making | COP31 Climate Negotiations | Group 9

---

## Repository structure

```
your-repo/
├── JUSTICE-main/                        ← clone the JUSTICE model here (see below)
├── caricom_justice_analysis_revised.ipynb
└── README.md
```

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
| Output 1 — Welfare function choice | Part 1 | printed output |
| Figure A — Temperature trajectories | Part 2 | `plots_caricom/caricom_01_temperature.png` |
| Figure B — Emissions vs damage share | Part 3 | `plots_caricom/caricom_02_damage_fraction.png` |
| Output 2 — Abatement burden vs damage  burden | Part 4a | printed output |
| Figure C — Abatement burden vs damage  burden | Part 4a | `plots_caricom/caricom_03_burden_comparison.png` |
| Output 3 — Abatement burden vs damage burden | Part 4b | printed output |
| Figure D — Abatement burden vs damage burden | Part 4b | `plots_caricom/caricom_new_01_injustice_ratio.png` |
| Figure E — Consumption per capita & the sufficiency floor | Part 5a | `plots_caricom/caricom_04_consumption_sufficiency.png` | 
| Figure F — Caribbean CPC trajectory (BAU vs high-ambition) | Part 5b | `plots_caricom/caricom_new_03_cpc_trajectory.png` |
| Output 4 — Scenario ensemble | Part 6 | printed output |
| Output 5 — Sensitivity analysis | Part 7 | printed output |
| Output 6 — Scenario discovery | Part 8 | printed output |
| Figure G — Scenario discovery | Part 8 | `plots_caricom/caricom_SD_scenario_discovery.png` |
| Figure H — Robustness by ECR | Part 9 | `plots_caricom/caricom_ROB_robustness.png` |
| Output 7 — Welfare function comparison | Part 10a | printed output |
| Figure I — Welfare function comparison | Part 10b | `plots_caricom/caricom_new_05_swf_regional_welfare.png` |
| Output 8 — Delta sensitivity | Part 11a | printed output |
| Figure J — Delta sensitivity | Part 11b | `plots_caricom/caricom_09_delta_sensitivity.png` |
| Output 9 — Debate evidence card | Part 12 | printed output |
| Figure K — Summary Figure | Part 13 | `plots_caricom/caricom_00_summary.png` |

All figures are saved automatically to a `plots_caricom/` folder created on first run.

---

## Key modelling choices

- **Welfare function:** Sufficientarian
- **Sufficiency threshold:** 75% of Caribbean CPC along a moderate-abatement (ECR = 0.3), no-damage-scaling reference trajectory under SSP3 — see Part 0 of the notebook for full justification
- **Ensemble:** 576 runs across SSP × ECS × δ × ECR
