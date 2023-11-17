# Evaluating the performance of polygenic risk scoring across diverse ancestry populations in Parkinson's disease 

`GP2 ❤️ Open Science 😍`

[![DOI](https://zenodo.org/)](https://zenodo.org/)

**Last Updated:** November 2023 

## Summary
This is the online repository for the manuscript titled ***"Evaluating the performance of polygenic risk scoring across diverse ancestry populations in Parkinson's disease"***.
This study aims to evaluate the multi-ancestry performance of predictive polygenic risk score (PRS) models using the 90 risk variants across 78 independent loci previously linked to Parkinson’s disease (PD) risk in the European population.

### Data Statement 
All data was using release 5 GP2 data (access-controlled via single-sign on on amp-pd.org) and 23andMe GWAS summary statistics (available via collaboration with 23andMe).

### Helpful Links 
- [medRxiv pre-print (November 2023)](https://www.medrxiv.org)
- [GP2 Website](https://gp2.org/)
    - [GP2 Cohort Dashboard](https://gp2.org/cohort-dashboard-advanced/)
- [Introduction to GP2](https://movementdisorders.onlinelibrary.wiley.com/doi/10.1002/mds.28494)
    - [Other GP2 Manuscripts (PubMed)](https://pubmed.ncbi.nlm.nih.gov/?term=%22global+parkinson%27s+genetics+program%22)


# Workflow Diagram 
![Workflow Diagram](https://github.com/GP2code/GP2-AFR-AAC-metaGWAS/blob/main/figures/PRS_Fig_1.png)




# Repository Orientation 
- The `analyses/` directory includes all analyses discussed in the manuscript
- The `figures/` directory includes all figures and supplemental figures referenced in the manuscript *(pending publication)*
- The `tables/` directory includes all tables and supplemental tables referenced in the mansucript *(pending publication)*

---
### Analysis Notebooks
* Languages: Python, bash, and R

| **Notebooks** |                                                    **Description**                                                   |
|:----------------:|:--------------------------------------------------------------------------------------------------------------------:|
|        00_PRS_release5_relatedness   | Estimate relatedness (filter for second-degree relationships) |
|        01_PRS_release5_summary_stats_meta  | Generate additive summary statistics for meta-GWASes with META (Base Data) Meta-GWAS #1: EAS (Foo + 23andMe) Meta-GWAS #2 AMR (Loesch + 23andMe)|  
|        02_PRS_release5_scores | Estimate Multi-ancestry PRS per ancestry (AAC, AFR, AJ, AMR, CAS, EAS, EUR)|
|        03_baseline_PRS_release5_regression_risk  | Estimate Multi-ancestry PRS versus PD risk per ancestry|
|        04_PCs_PRS_release5_regression_risk  | Estimate Multi-ancestry PRS versus PD risk adjusted by covariates per ancestry (age, gender, PCs)|
|        05_admixture_PRS_release5_regression_risk  | Estimate Multi-ancestry PRS versus PD risk adjusted by covariates per ancestry (age, gender, % admixture)|
|        06_data_visualization | Generating density, forest, ROH plots per ancestry|
|        07_PRS_release5_regression_age_at_onset    | Estimate Multi-ancestry PRS versus age at onset |
|        08_Specificity_Sensitivity  | Estimate Specificity and Sensitivity |
|        09_PRS_release5_Table1 | Generate Table 1 |
|        10_PRS_release5_power_calculations_age_at_onset.R | Estimate power for age at onset |
|        11_PRS_release5_power_calculations_disease_status.R | Estimate power for disease status |

---
### Figures and Supplemental Figures

*(pending publication)*

---
### Tables and Supplemental Tables 

*(pending publication)*

---

# Software 
                             
|               Software              |      Version(s)     |                       Resource URL                       |       RRID      |                                               Notes                                               
|:-----------------------------------:|:-------------------:|:--------------------------------------------------------:|:---------------:|:------------------------------------------------------------------------------------:|

|                METAL                |      2020-05-05     |         http://csg.sph.umich.edu//abecasis/Metal/        | RRID:SCR_002013 |                                       used for meta-analyses                          
|                PLINK                | 1.7 and 1.9 and 2.0 |            http://www.nitrc.org/projects/plink           | RRID:SCR_001757 |                                     used for genetic analyses                         
|     Python Programming Language     |     3.8 and 3.9     |                  http://www.python.org/                  | RRID:SCR_008394 | pandas; numpy; seaborn; matplotlib; statsmodel; used for general data management|
| R Project for Statistical Computing |         4.2         |                 http://www.r-project.org/                | RRID:SCR_001905 | tidyverse; dplyr; tidyr; ggplot; data.table; used for general data management|
