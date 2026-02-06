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

- Of note, the data was obtained from FITBIR and requires approval for access. Those data have been removed from this repository, but are available for request here: https://fitbir.nih.gov/content/access-data

- Data used from this analysis are from Zafonte et al. (2012), with the Citicoline group removed to only include healthy controls.
- Zafonte, R. D., Bagiella, E., Ansel, B. M., Novack, T. A., Friedewald, W. T., Hesdorffer, D. C., Timmons, S. D., Jallo, J., Eisenberg, H., Hart, T., Ricker, J. H., Diaz-Arrastia, R., Merchant, R. E., Temkin, N. R., Melton, S., & Dikmen, S. S. (2012). Effect of citicoline on functional and cognitive status among patients with traumatic brain injury: Citicoline Brain Injury Treatment Trial (COBRIT). JAMA, 308(19), 1993–2000. https://doi.org/10.1001/jama.2012.13256



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
