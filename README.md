# Regional and Temporal Variation in Coal Power's Emission Intensity (2000–2024)

**Author:** Logan Rosell\
**Affiliation:** School of Computing & Information Sciences, Willamette University\
**Course:** Data501: Data Science With R (Instructor: Dr. Zechariah Meunier)

------------------------------------------------------------------------

## Overview

This repository analyzes whether coal-fired power generation's CO2 emission intensity (mtCO2/TWh) varies across global regions and over time from 2000 to 2024. Using yearly electricity generation and emission data from [Ember](https://ember-energy.org/data/yearly-electricity-data/), this project explores regional disparities, evaluates temporal efficiency improvements, and investigates the limits of intensity gains compared to overall capacity reduction.

## Key Findings

-   **Regional Differences:** Non-parametric testing (Kruskal-Wallis and pairwise Wilcoxon rank-sum tests) shows statistically significant differences in median CO2 emission intensity across all seven world regions (p \< 0.01).
-   **Temporal Trends:** While global linear models suffer from severe collinearity and non-linearities, region-specific models identify statistically significant declines in CO2 intensity over time in **Asia** (R\^2 = 0.94) and **Oceania** (R\^2 = 0.86).
-   **Impact Context:** While efficiency improvements in Asia prevented an estimated 14.68 million metric tons of CO2 in 2024, this represents only \~0.18% of the region's total coal power emissions, demonstrating that phasing out coal capacity remains far more impactful than incremental plant-level efficiency gains.

## Repository Structure

``` text
├── data/
│   └── yearly_full_release_long_format.csv   # Raw Ember electricity data (2000–2024)
├── outputs/
│   └── plots/                               # Exported figures, maps, and tables
├── scripts/
│   └── global_power_r_final_content.Rmd     # Analysis, data cleaning, and modeling
├── coal_power_co2_intensity_repo.Rproj       # RStudio project configuration
└── .gitignore
```
