# Predicting Test Scores for High School Students

## Overview
This project uses linear regression models to predict test scores in reading, math, and writing among a cohort of 948 high school students. Six candidate models, all using OLS regression were proposed, either based on underlying hypotheses or model selection procedures.

## Data
- **Source:** Columbia University (P8130: Biostatistical Methods I course materials)
- **Sample size:** 948 high school students
- **Response variable:** Reading, Math, and Writing test scores
- **Predictors:** Demographic variables, parent education status, parent marital status, birth order, weekly study hours, transportation method to school

## Methods
- Data preprocessing and exploratory analysis in R
- Feature exploration of response and predictors
- OLS Regression to predict a continuous outcome
- Diagnostic plots, including residual plots and Q-Q plots, for final model

## Results
- Backward selection model achieved the highest R^2, more so than any of the theoretical (economic, hard worker, demographic, family structure) models
- Still, none of the models were particularly predictive of test scores (max R^2 = 0.33)

Selected visualizations are available in the accompanying PDF report and the `output/` directory.

## Limitations and Future Work
- Lack of data on type of school students attended (i.e. public/charter/private)
- Given that the sample is of high school students, larger sample size could be achieved

## Reproducibility
All analyses were conducted in R. The R Markdown file contains code to preprocess the data,
train models, and evaluate performance using the `caret`, `kernlab`, and `ggplot2` packages.
