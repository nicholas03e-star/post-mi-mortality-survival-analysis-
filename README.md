Post-MI Mortality: Survival Analysis & Risk Stratification
Survival analysis of post-myocardial infarction (MI) mortality using the WHAS500 dataset (500 patients, Worcester Heart Attack Study).
Methods

Log-rank tests for univariate screening of binary covariates (afb, chf, cvd, gender, miord, mitype, sho)
Cox Proportional Hazards model with proportionality assumption testing via Schoenfeld residuals
Stratified Cox PH to handle variables violating the PH assumption (shock status, MI type)
Weibull AFT model for parametric survival estimation and acceleration factor computation
Clinical subgroup risk quantification via AFT acceleration factors

Key Findings

LOS (length of stay) excluded from model — post-outcome variable creating circularity
Shock status (sho) and MI type (mitype) required stratification after PH assumption testing
AFT acceleration factors computed to quantify differential survival time across clinical subgroups

Dataset
WHAS500 — Worcester Heart Attack Study, 500 patients, available via scikit-survival
Dependencies
scikit-survival
lifelines
pymc
pytensor
arviz
scipy
numpy
pandas
matplotlib
statsmodels
Install with:
bashpip install scikit-survival lifelines pymc arviz
Files

survival_analysis.ipynb — Full analysis noteboo
