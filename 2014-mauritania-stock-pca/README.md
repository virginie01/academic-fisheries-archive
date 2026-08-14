# Multivariate Stock Community Analysis: Mauritania Demersal Fisheries (1982–2006)

This subdirectory contains the case study and analytical methodology for a large-scale stock community analysis conducted at Agrocampus Ouest in January 2014 under the academic supervision of Dr. François Husson.

---

## Subdirectory Materials
* **Full Academic Report:** [View the PDF Report](./Mauritania_Fisheries_Stock_Report_2014.pdf) *(Written in French)*
* **Code Implementation:** Full data cleaning loops, standardized PCA configurations, and HCPC clustering scripts using the `FactoMineR` package are documented in the **Appendices (Annexes)** at the end of the report document.

---

## Core Methodological Keywords
* **Multivariate Statistics:** Standardized Principal Component Analysis (PCA), Hierarchical Clustering on Principal Components (HCPC), Ward's Ascendant Hierarchical Method.
* **Fisheries Ecology:** Catch Per Unit Effort (CPUE / PUE - Prise par Unité d'Effort), Demersal Species Assemblages, Bathymetric Gradients, Spatio-Temporal Structuring.
* **Data Processing:** Interannual Averaging, Sparse Data Filtering.

---

## Study Objectives & Technical Framework

### 1. Data Pipeline & Data Reduction
The initial database comprised **34,185 distinct catch records** collected during scientific trawling campaigns off the coast of Mauritania spanning from 1982 to 2006. To eliminate noise from rare species while preserving community signals, the framework compressed **565 observed species down to 26 core target indicator species** based on a strict dual filter:
* An organism must be observed > 200 times across campaigns.
* The species must maintain a mean localized abundance metric > 1.

Interannual averaging was executed across spatial and seasonal criteria to isolate permanent structural environmental signals from volatile year-to-year variation, yielding 52 distinct spatio-temporal statistical individuals.

### 2. Multivariate Analysis & Clustering
Using the `FactoMineR` ecosystem, a standardized PCA was deployed to evaluate community correlations across 4 dimensions (accounting for over 50% of the total dataset variance). To validate the resulting coordinate clouds, an agglomerative hierarchical classification (HCPC) was executed using **Ward's minimum variance criterion** to group the species into 5 distinct ecological community clusters.

### 3. Key Scientific Findings
* **Bathymetric Dominance:** The model mathematically isolated **bathymetry (depth strata) as the primary organizing factor** behind Mauritanian fish communities. Clear divisions map coastal species assemblages (Strata 1 & 2: 0–50m, characterized by *Epinephelus aeneus* and *Decapterus rhonchus*) apart from deep-water communities (Strata 5: >200m, dominated exclusively by *Brotula barbata* and *Halobatrachus didactylus*).
* **Macro-Scale Latitudinal Gradients:** Dimensions 3 and 4 successfully mapped a clear geographic gradient, identifying significant community shifts between Northern and Southern Mauritanian boundaries.
* **Seasonal Invariance:** The analysis proved that seasonal variations (cold, warm, and transitional periods) had **no statistically significant correlation** with broad community structure, suggesting that depth preferences remain stable throughout the year.

---

## Contributors & Citation Context
* **Authors:** J. Benoit, V. Bornarel
* **Academic Institution:** Agrocampus Ouest, Department of Fisheries and Aquaculture (*Département Halieutique*), 2014.
* **Supervisor:** Dr. François Husson

*Disclaimer: This project functions strictly as a historical portfolio reference showcasing foundational training in multivariate statistics and community ecology frameworks.*
