# Discretisation of Spatial Point Data: Pixel Size Effects in Mineral Prospectivity Analysis

## Overview
Investigated how pixel size selection affects logistic regression parameter estimates 
in spatial mineral prospectivity analysis, using the Murchison gold deposit dataset 
from Western Australia. The Poisson Point Process (PPP) was used as a theoretical 
benchmark, with logistic regression models compared across 100 pixel sizes in the 
1–3km range.

Supervised by Dr Suman Rakshit — Curtin University, 2026.

## Tools & Technologies
- R (spatstat, ggplot2)
- Poisson Point Process modelling (Berman-Turner device)
- Spatial logistic regression (slrm)
- ROC curve analysis

## Key Findings
- AUC values exceeded 0.91 across all pixel sizes, indicating strong discriminative 
  performance regardless of resolution
- Logistic regression estimates closest to the PPP benchmark in the 2–2.5km pixel 
  size range — providing a practical recommendation for industry practitioners
- Rule S discretisation produced estimates closer to the PPP benchmark on average, 
  but with substantial oscillation driven by boundary misclassification of the binary 
  greenstone covariate
- Rule R discretisation significantly reduced instability, confirming findings from 
  Baddeley et al. (2025), but produced estimates sitting further from the PPP 
  benchmark — revealing a stability vs accuracy trade-off

## How to Run
1. Open `Industrial Project V1.Rmd` in RStudio
2. Ensure the `spatstat` and `ggplot2` packages are installed
3. Knit the document to reproduce the full analysis

## References
Baddeley et al. (2025) — *Mineral Prospectivity Analysis Is Unstable to Changes 
in Pixel Size*, Computers and Geosciences.
