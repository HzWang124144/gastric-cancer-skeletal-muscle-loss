# gastric-cancer-skeletal-muscle-loss
# Early prediction of skeletal muscle loss in gastric cancer

This repository contains the de-identified minimal dataset and supporting files for the study:

**Early prediction of skeletal muscle loss using longitudinal clinical data in patients with gastric cancer after radical gastrectomy and adjuvant chemotherapy: a retrospective cohort study**

## Overview

This study developed and evaluated machine learning models for early prediction of significant skeletal muscle loss in patients with gastric cancer who underwent radical gastrectomy followed by adjuvant chemotherapy.

The outcome was defined using computed tomography (CT)-based skeletal muscle index (SMI) changes between baseline and follow-up imaging. Candidate predictors included baseline clinical variables, laboratory and tumor marker data, inflammatory/nutritional indicators, and early postoperative longitudinal dynamic features.

The final model identified in the study was a multilayer perceptron (MLP) model.

## Repository contents

- `data/`
  - De-identified minimal dataset used for analysis
- `codebook/`
  - Variable definitions and coding information
- `analysis/` *(optional)*
  - Scripts used for preprocessing, model development, and evaluation
- `README.md`
  - Project description and data documentation

## Data description

The dataset includes de-identified clinical variables from patients with gastric cancer treated with radical gastrectomy and adjuvant chemotherapy.

### Main variable categories

- Demographic characteristics  
  - sex
  - age
  - body mass index (BMI)

- Tumor-related variables  
  - histologic grade
  - tumor location
  - operation type
  - T stage
  - N stage

- Laboratory and tumor marker variables  
  - red blood cell count (RBC)
  - hemoglobin (HGB)
  - lactate dehydrogenase (LDH)
  - homocysteine (HCY)
  - carcinoembryonic antigen (CEA)
  - carbohydrate antigen 19-9 (CA199)
  - carbohydrate antigen 72-4 (CA724)

- Inflammatory and nutritional indicators  
  - neutrophil-to-lymphocyte ratio (NLR)
  - leukocyte-to-lymphocyte ratio (LLR)
  - platelet-to-lymphocyte ratio (PLR)
  - systemic immune-inflammation index (SII)
  - prognostic nutritional index (PNI)

- Longitudinal dynamic features  
  - ΔRBC
  - ΔNLR
  - ΔLLR
  - ΔPLR
  - ΔPNI
  - ΔSII
  - ΔLDH
  - ΔHCY

## Outcome definition

Significant skeletal muscle loss was defined as a decrease of at least 5% in skeletal muscle index (SMI) between:

- baseline CT performed within 2 weeks before surgery, and
- follow-up CT obtained 3 months after initiation of adjuvant chemotherapy.

Patients were classified into:

- `1` = skeletal muscle loss
- `0` = skeletal muscle maintenance

## Variable notes

- `Δ` indicates the relative change from baseline to 1 month after surgery.
- Details of variable definitions are provided in the codebook file.

## Data availability

This repository provides the de-identified minimal dataset underlying the findings of the study. All personal identifiers were removed before data sharing.

## Citation

If you use this dataset, please cite the associated article:

> [Add full citation here after publication]

## Contact

For questions regarding the dataset, please contact:

**Zhongchuan Lv**  
Department of General Surgery  
The Affiliated Yantai Yuhuangding Hospital of Qingdao University  
Yantai, Shandong, China  
Email: wanghanzheng000@163.com

## Disclaimer

These data are shared for research and academic use only. Users are responsible for appropriate use and interpretation of the dataset.
