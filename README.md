# mineral-prospectivity-analysis

## Overview
Investigated how pixel size selection affects parameter estimates in logistic regression models for spatial mineral prospectivity analysis, using the Murchison gold deposit dataset in Western Australia.

## Tools & Technologies
- R (spatial analysis, statistical modelling)
- Packages: spatstat, ggplot2
- Logistic regression, Poisson Point Process models
- ROC curve analysis

## Methodology
- Fitted Poisson Point Process models as a theoretical benchmark
- Compared against logistic regression models across 100 different pixel sizes
- Evaluated two discretisation rules and assessed model performance via ROC curve analysis

## Key Findings
- Achieved AUC values above 0.93 across fine-resolution models
- Identified 2–2.5km as the optimal pixel size range, balancing aggregation bias and numerical instability
- Provides a practical recommendation for industry practitioners in mineral exploration

## How to Run
1. Open `Industrial Project V1.Rmd` in RStudio
2. Install required packages if needed
3. Knit the document to generate the full analysis output
