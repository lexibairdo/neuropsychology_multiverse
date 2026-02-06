## Neuropsychology Multiverse Analysis

This repository contains the data and code for Into the Multiverse: Applications to Neuropsychology, by C. Lexi Baird, Hollie A. Mullin, and Frank Hillary.

Here, we demonstrate how a multiverse approach can be applied to examine outcomes following complicated mild and moderate-to-severe traumatic brain injury (TBI). We evaluate the outcome of distinct methodological choices, including variation in covariates, TBI severity predictors, and outcome measures, to investigate our research questions. We also provide practical guidance for organizing and presenting results when faced with a
large number of model specifications. Although TBI serves as our test case, the primary goal is to highlight the broader applicability of multiverse methods in the clinical
neurosciences. 

The analyses are implemented in R using the **`specr`** package (https://masurp.github.io/specr/) to generate specification curve figures. 

Masur, Philipp K. & Scharkow, M. (2020). specr: Conducting and
Visualizing Specification Curve Analyses. Available from
https://CRAN.R-project.org/package=specr.

---

## Repository contents

- **`multiverse_analysis.qmd`**: Main Quarto document that runs the multiverse/specification-curve analyses and exports figures and summary tables.
- **`multiverse_analysis.html`** and **`docs/`**: Rendered report and website-ready version (can be served via GitHub Pages).
- **Data files**:
  - **`mv_complete.xlsx`**: Analysis-ready dataset (complete cases for variables of interest).
  - **`multiverse_merged.csv`**: Source multiverse dataset (before filtering to Placebo and complete cases).
  - **`GOSE_GCS_extended_appendix.csv`**: GOSE/GCS appendix used to derive TBI severity and PTA measures.


### 1. Software requirements

- **R** (version 4.x recommended)
- **Quarto** (for rendering the `.qmd` document to HTML/Word)

R packages (install as needed):

```r
install.packages(c(
  "stringr", "lavaan", "readxl", "dplyr", "tidyr",
  "lme4", "ggplot2", "writexl"
))

# specr is available on CRAN; if not present, install from GitHub:
install.packages("specr")
```
