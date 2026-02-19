# Solar Ingot Puller Process Stability & Risk Analytics

## Business Context

Crystal growth processes such as solar ingot pulling operate under tightly
coupled thermal, mechanical, and control constraints. Small instabilities in
process behavior can propagate into significant quality and yield risks.

This project demonstrates a structured analytics approach to quantify process
stability, identify high-risk operating regimes, and isolate interpretable risk
drivers using equipment telemetry data.

## Data Confidentiality

This repository uses fully synthetic and anonymized data for public
demonstration. All values, timestamps, and identifiers are artificially
generated and do not correspond to any real equipment or production process.

The analytics workflow, feature engineering strategy, and modeling logic are
identical to those applied on proprietary industrial datasets.

## Methodology Overview

The analysis follows a structured, production-oriented workflow:

1. Structured ingestion and schema understanding of puller telemetry
2. Engineering of control deviation (SP–PV gaps), rolling variability, and drift features
3. Construction of a composite Stability Index to quantify short-term instability
4. Segmentation of Stable vs High-Risk operating regimes
5. Comparative analysis to identify concentrated instability drivers
6. Regression-based validation using interpretable logistic models
7. 
## Repository Structure

notebooks/
- 01_data_loading_understanding.ipynb
- 02_data_cleaning_feature_engineering.ipynb
- 03_process_stability_risk_analysis.ipynb
- 04_regression_validation.ipynb

data/
- synthetic/   # anonymized demonstration data only
- 
## Key Insights

- Process instability is driven primarily by short-term variability and control
  deviation rather than mean shifts alone.
- High-risk behavior is concentrated in a small subset of interpretable process
  parameters, enabling targeted control improvement.
- Rolling variability metrics provide earlier and more sensitive indicators of
  instability than traditional average-based monitoring.
- Regression validation confirms that engineered features systematically explain
  elevated process risk.
  
## Tools & Skills

- Python (pandas, numpy, scikit-learn, matplotlib)
- Time-series feature engineering
- Process stability & risk analytics
- Interpretable regression modeling
- Industrial data anonymization & governance

