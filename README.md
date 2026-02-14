# Glucose Levels Statistical Analysis

Statistical analysis of glucose tolerance test data investigating whether glucose tolerance decreases with age.

The study compared two groups of healthy patients:
- Young group (under 30 years)
- Adult group (over 30 years)

Blood glucose was measured at two points: baseline (immediately after glucose intake) and 60 minutes post-intake.

## Analysis Performed

### Descriptive Statistics
- Calculated central tendency and dispersion measures for both groups' baseline glucose levels
- Evaluated representativeness of means using coefficient of variation
- Analyzed skewness and kurtosis for adult baseline glucose
- Generated quartiles and box plots for young group, identifying outliers
- Tested normality of 60-minute glucose data for both groups using Shapiro-Wilk test

### Correlation and Regression
- Examined linear relationship between baseline and 60-minute glucose in young group
- Calculated Pearson correlation coefficient (r = 0.796, p < 0.001)
- Developed linear regression model: 60-min glucose = 0.697 × baseline + 91.384
- Model explains 63.4% of variability (R² = 0.634) with RMSE of 4.61 mg/dL
- Predicted 60-minute glucose for baseline value of 83 mg/dL: 149.23 mg/dL

### Hypothesis Testing
- Tested whether mean baseline glucose in young people equals 88 mg/dL (95% and 99% confidence intervals)
- Compared means between young and adult groups using Welch's t-test (p = 0.022)
- Analyzed proportion of patients with prediabetic levels (>95 mg/dL) using 98% confidence interval
- Performed paired samples test for adult group to detect glucose variation between measurements

## Key Findings

- Adults show significantly higher baseline glucose levels than young people (difference: 0.7 to 8.7 mg/dL)
- Strong positive correlation exists between baseline and 60-minute glucose in young subjects
- Linear regression provides reasonable prediction accuracy for 60-minute glucose
- Glucose levels in adults increase approximately 82 mg/dL on average after 60 minutes
- Data supports the hypothesis that glucose tolerance decreases with age

## Technologies Used

- Python (Pandas, NumPy)
- Statistical analysis (SciPy)
- Machine learning (Scikit-learn)
- Data visualization (Matplotlib, Seaborn)

## Files

- `glucose_levels.ipynb`: Complete analysis with code and documentation
- `glucose_sample.xlsx`: Dataset containing 65 patient records