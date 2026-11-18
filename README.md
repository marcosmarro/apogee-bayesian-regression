## APOGEE (Stellar Spectra) Analysis
### Data Source
* Sloan Digital Sky Survey (SDSS).

### Focus
* Analyzing near-infrared stellar spectra to understand the chemical composition of the Milky Way.

### Methodology
* **Beyond Point Estimation:** Analyzed why standard Maximum Likelihood Estimation (MLE) leads to overconfident predictions and underestimates error due to overfitting.
* **Bayesian Linear Regression:** Implemented a model that accounts for:
    * **Heteroscedastic Noise:** Varying measurement errors across different stellar temperatures.
    * **Parameter Uncertainty:** Using a posterior distribution of weights rather than a single fixed value.
* **Hyperparameter Tuning:** Evaluated the impact of the prior strength (2) on model flexibility and regularization.

### Calibration & Performance
* **RMSE:** Achieved a Root Mean Square Error of **166.4 K**.
* **Coverage Statistics:** Used coverage (the percentage of actual values falling within the 95% Confidence Interval) to evaluate model calibration.
* **Optimal Result:** With 2=105, the model achieved a coverage of **0.967**, indicating a highly calibrated and reliable predictive model.
