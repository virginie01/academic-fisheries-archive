# Bayesian Life-Cycle Modeling of Atlantic Salmon

This repository serves as a methodological archive and case study for a quantitative fisheries research project completed in February 2016 at Agrocampus Ouest. It implements an integrated population dynamics framework to analyze environmental and anthropogenic drivers of Atlantic Salmon (*Salmo salar*) decline across the North American Atlantic coast.

---

## Project Materials & Navigation
* **Full Academic Report:** [View the PDF Report](./North_American_Salmon_Bayesian_Report_2016.pdf) *(Written in French)*
* **Code Implementation:** Complete `rjags` and `FactoMineR` baseline modeling scripts, parameter specifications, and MCMC initialization architectures are fully documented in the **Appendix (Annexe)** at the end of the report document.

---

## Core Methodological Keywords
* **Modeling Frameworks:** Hierarchical Bayesian Models (HBM), State-Space Population Dynamics, Integrated Life-Cycle Modeling.
* **Statistical Methods:** Multi-Regional Covariance Mapping, Principal Component Analysis (PCA), Hierarchical Clustering, Markov Chain Monte Carlo (MCMC) Simulations.
* **Management & Policy:** Management Strategy Evaluation (MSE), Conservation Limits (CL), Quota Policy Simulations, Stochastic Projections.
* **Software Tech Stack:** R, RJAGS / JAGS (Just Another Gibbs Sampler), FactoMineR.

---

## Scientific Summary & Project Architecture

Using 40+ years of historical data (1970–2013)—including river counts, marine catches, and biological traits across 6 North American salmon management zones (spanning from the United States to Labrador)—this project built iterative state-space models to evaluate spatial synchrony in salmon demographic traits and simulate future management choices.

The modeling framework was developed across four progressive cycles to handle complex observation and process errors:

1. **Cycle 0 (Baseline):** A foundational random-walk model mapping a single sea-winter (2SW) lifecycle branch for a isolated region (Newfoundland) to establish baseline parameters.
2. **Cycle 1 (Demographic Complexity):** Integration of early maturation branches to separate and track 1SW vs. 2SW migration routing and return rates.
3. **Cycle 2 (Anthropogenic Pressures):** Incorporation of marine catch and harvest metrics to mathematically isolate human fishing pressures from natural environmental marine mortality.
4. **Cycle 3 (Multi-Regional Scaling):** Expansion into a multi-regional independent and dependent covariance matrix framework. Comparison between a full regional covariance formulation and a model decomposing variation into synchronous and asynchronous components, with an ICC-type index quantifying the proportion of inter-annual variation attributable to the shared signal. Using Principal Component Analysis (PCA), this phase evaluated spatial synchrony, proving that population variations were highly synchronized across 5 out of the 6 geographic zones.

### Management Strategy Evaluation (MSE)
The final phase of the project ran 5-year population trajectory outlooks under varying harvest control rules (Status Quo, Total Moratoria, and Targeted Quotas). The outputs simulated the mathematical probability of these populations meeting or maintaining ICES and NASCO conservation thresholds under shifting environmental regimes.

---

## Authors
* **Collaborators:** V. Bornarel, P.-Y. Hernvann, C. Le Guen, and A. Schickele
* **Institutional Context:** Agrocampus Ouest, 2016.

*Disclaimer: This repository functions strictly as a historical portfolio reference showcasing foundational training in Bayesian stock assessment and state-space modeling structures. The original materials represent collective group outputs from an academic curriculum.*
