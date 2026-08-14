# Historical Fisheries Archive: Bayesian population dynamics & Multivariate community analysis

This repository serves as a centralized methodological archive and portfolio showcasing quantitative research projects completed during my Master's curriculum at Agrocampus Ouest. These case studies demonstrate a long-standing track record in advanced fisheries data science, multivariate community analysis, and Bayesian population dynamics.

---

## Repository Architecture & Navigation

```text
├── README.md                           
├── 2014-mauritania-stock-pca/
│   ├── Mauritania_Fisheries_Stock_Report_2014.pdf
│   └── README.md                      
└── 2016-salmon-lifecycle-hbm/
    ├── North_American_Salmon_Bayesian_Report_2016.pdf
    └── README.md                      
```

### Accessing Materials & Code Snippets
* **Project Reports:** The full reports are available as standalone PDFs within their respective project directories *(both written in French)*.
* **Code Implementation:** Full software configurations, matrix initializations, and model scripts are completely documented inside the **Appendices (Annexes)** at the end of each respective PDF report.

---

## Core Technical Keywords
* **Statistical Modeling:** Hierarchical Bayesian Modeling (HBM), State-Space Dynamics, Markov Chain Monte Carlo (MCMC) Simulations.
* **Multivariate Analytics:** Principal Component Analysis (PCA), Hierarchical Clustering on Principal Components (HCPC), Ward's Clustering, Community Ecology.
* **Fisheries Management:** Catch Per Unit Effort (CPUE/PUE), Stock Assessments, Management Strategy Evaluation (MSE), Harvest Control Rule Simulations.
* **Software Tech Stack:** R, JAGS / RJAGS, FactoMineR.

---

## Project Case Studies

### 1. Bayesian Life-Cycle Modeling: Atlantic Salmon Decline
* **Directory:** `/2016-salmon-lifecycle-hbm`
* **Core Objective:** Disentangle anthropogenic fishing pressures from natural marine environmental mortality across 6 North American management regions spanning a 40+ year timeline (1970–2013).
* **Methodology:** Implemented an integrated state-space population dynamic framework using multi-regional independent and dependent covariance matrices. The framework used logit-scale random walks to model shifting temporal variations in post-smolt survival vs. maturation schedules. 
* **Key Finding:** PCA verified macro-scale marine environmental synchrony across 5 out of 6 geographic management zones, concluding with a 5-year stochastic forecast simulating population limits under varying international harvest control quotas.

### 2. Multivariate Community Analysis: Mauritania Demersal Fisheries
* **Directory:** `/2014-mauritania-stock-pca`
* **Core Objective:** Identify distinct marine species assemblages and evaluate spatio-temporal drivers of stock structuring off the coast of Mauritania.
* **Methodology:** Processed a large-scale database comprising 34,185 catch records spanning 1982 to 2006. Computed Catch Per Unit Effort (CPUE/PUE) indices for 26 target indicator species. Applied standardized PCA and HCPC (using Ward's clustering criterion) to identify distinct population classes.
* **Key Finding:** Successfully mapped a strict bathymetric gradient across five distinct depth layers (0m to >200m). The model proved that depth-strata configurations dictate community assemblages more strongly than localized latitudinal zones or seasonal transitions.

---

## Project Contributors & Context
* **2016 Salmon Project Co-Authors:** V. Bornarel, P.-Y. Hernvann, C. Le Guen, A. Schickele.
* **2014 Mauritania Project Co-Authors:** J. Benoit, V. Bornarel.
* **Academic Institution:** Dept. Halieutique, Agrocampus Ouest.
* **Academic Supervision (2014):** Dr. François Husson *(Co-creator of the FactoMineR R Package)*.

*Disclaimer: This repository functions strictly as a historical portfolio reference showcasing early professional training in quantitative fisheries science. All scripts and reports are presented as unmaintained, historical academic artifacts.*
