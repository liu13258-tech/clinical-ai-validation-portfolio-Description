# Clinical AI Model Validation Portfolio

## Overview
This repository demonstrates an end-to-end clinical AI validation workflow using
probability-based model outputs. The focus is on clinically meaningful evaluation,
including threshold selection, confusion-matrix–derived metrics, and subgroup analysis,
rather than relying on default thresholds or single performance scores.

## Clinical Context
The model is evaluated under a screening-style use case, where minimizing false negatives
is prioritized due to patient safety considerations. All operating points are selected
based on clinical risk trade-offs.

## Key Components
- **Data exploration**: Understanding model outputs and ground truth labels
- **Confusion matrix analysis**: Manual derivation of TP, TN, FP, FN and related metrics
- **Threshold sweeping**: Sensitivity–specificity trade-off analysis across operating points
- **ROC/AUC analysis**: Assessment of overall discrimination ability
- **Subgroup analysis**: Evaluation of robustness across simulated acquisition devices

## Project Structure
clinical-ai-validation-portfolio/
├── README.md
├── notebooks/
│ ├── 01_data_exploration.ipynb
│ ├── 02_confusion_matrix_hand_calc.ipynb
│ ├── 03_threshold_sweeping.ipynb
│ ├── 04_roc_auc.ipynb
│ └── 05_subgroup_analysis.ipynb
## Key Takeaway
Clinical AI deployment decisions should be driven by patient safety and clinical risk,
not by default thresholds or single performance metrics.

## Notes
All data used in this repository are synthetic and intended solely for demonstration
of clinical AI validation concepts.
