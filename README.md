# UCSD Parking Occupancy Analysis

A statistical inference project (DSC 190) testing whether parking occupancy differs meaningfully across permit types on UCSD's campus, using real occupancy data and a stakeholder-facing deliverable for UCSD Transportation Services.

**My role:** led this project with Seiichi Nakahira (collaborative, 2-person project) — I drove most of the analysis and the stakeholder-facing presentation.

## What it does

Analyzes 1,071 peak-hour occupancy observations (20 years of data) across all UCSD parking structures and 5 permit types, using one-way ANOVA and a 3,000-shuffle permutation test to check whether the observed differences in occupancy between permit types are statistically meaningful rather than noise.

## Results

- **F = 25.52, p < 0.001** — occupancy differs significantly by permit type, confirmed by permutation test
- Resident-student parking is near saturation (**97.5% mean occupancy**) vs. **87.6%** for commuter-student parking
- Findings were presented directly to the **UCSD Transportation Services President**

## Stack

Python (pandas), one-way ANOVA, permutation testing, Jupyter

## Data note

Includes a permit/capacity file provided directly by UCSD Transportation Services for this analysis (`Consolidated Fall 2025 QPass...xlsx`) alongside weekly occupancy snapshots. Aggregate occupancy figures only — no individual-level data.

## Run it locally

Open `Final_Report.ipynb` (or `Final_Report_Code.ipynb` for the code-only version) in Jupyter. `data_importing.ipynb` and `parking_q1_preparation.ipynb` show the earlier data-cleaning steps.
