## Disclaimer
This repository contains no real patient data.

## Predicting Progression from Early to Advanced Systemic Sclerosis
This exploratory cohort study aimed to determine the time to progression from early symptoms to established Systemic Sclerosis (SSc), and to identify which early autoantibody profiles and clinical symptoms are most associated with progression. The ultimate goal is to improve early diagnosis and guide treatment decisions.

## Goals and Purpose of the Project
Systemic Sclerosis is a rare but severe autoimmune disease. Early identification of patients at high risk of progression is crucial for timely treatment and improved outcomes. This project supports clinicians by identifying prognostic markers that can guide decision-making in early-stage patients.

## Approach
- Retrospective cohort design
- Kaplan-Meier analysis for cumulative incidence
- Log-rank tests for group comparisons
- Cox regression for hazard ratios
- Stratification by autoantibody profile, capillary density, telangiectasia, age, and sex

## Data Cleaning & Filtering
- **Exclusion criteria**: Patients with established SSc or missing consent were removed.
- **Missing data handling**:
  - Capillary density data was available for 53 patients.
  - NCM mean capillary density values were available for 53 patients.
- **Standardization**:
  - RP and PF duration were standardized to months using fixed conversion rules.
  - Autoantibody profiles were grouped into ACA, ATA, other ENAs, and ENA-negative.
  - Capillary density was categorized as ≤ 7 (significant loss) or > 7.
  - Age was stratified into three groups: 20–45, 45–60, and 60+ years.
- **Derived variables**:
  - Progression was defined by meeting ≥1 of the following: mRSS > 0, internal organ involvement, or start of immunosuppressive therapy.

## Technologies
- **R**: Statistical analysis and visualization
- **SDTM**: Standardization of clinical data
- **Epic-system**: Extraction of clinical data from consented patients
- **Castor EDC**: Data collection and management

## Data
**Source**: Patient data from the Radboudumc collected between 2017 and 2023. Initial sample size: 87 patients; final sample size: 62 patients  
  - 20 for not meeting the baseline criteria for early-stage systemic sclerosis  
  - 5 excluded due to missing consent
<img width="300" height="763" alt="image" src="https://github.com/user-attachments/assets/7fb584f6-50da-4ea3-af33-d49b550ea4df" />

*Figure 1. Flow chart of patient selection*


The dataset includes both clinical and immunological baseline characteristics:

| Category              | Variables                                                                 |
|-----------------------|---------------------------------------------------------------------------|
| Demographics          | Age, Sex                                                                  |
| Lifestyle             | Smoking status (current and ever smoked)                                  |
| Clinical Symptoms     | Raynaud's phenomenon (RP), Puffy fingers (PF), Telangiectasia             |
| Microvascular         | Nailfold capillary density, Nailfold capillaroscopy (NCM) pattern         |
| Immunological         | ANA positivity, ENA profile (ACA, ATA, other ENAs, ENA-negative)          |
| Inflammation          | Erythrocyte Sedimentation Rate (ESR)                                      |
| Disease Progression   | Modified Rodnan Skin Score (mRSS), internal organ involvement, treatment  |

## Results & Visuals
<img width="450" height="519" alt="image" src="https://github.com/user-attachments/assets/bc1e8242-fd83-42bc-a8d9-4011bff1168f" />

*Figure 2. Cumulative incidence function for progression, including 95% CI (n=62)*

**Median progression time**: 2.82 years

**Significant predictors**:
  - Telangiectasia (HR 2.17, p = 0.021)
  - Nailfold capillary density ≤ 7 (HR 3.62, p < 0.001)
  - ENA autoantibody profile (p = 0.009)

<img width="320" height="443" alt="image" src="https://github.com/user-attachments/assets/ec6fec3d-c922-4d3e-9125-22683a84d41d" /> <img width="320" height="442" alt="image" src="https://github.com/user-attachments/assets/9cb9d834-4528-438d-bd1b-7145bdc03dcc" />

<img width="310" height="443" alt="image" src="https://github.com/user-attachments/assets/e8b09252-f314-4111-b823-e12e488bfa43" />

*Figure 4. Cumulative incidence function by telangiectasia status*
*Figure 5. Cumulative incidence function by NCM mean capillary density divided into ≤ 7 and > 7*
*Figure 3. Cumulative incidence function by ENA status*

All visualizations and results are available in the full report (PDF)

## Status
Completed  
Internship period: Feb 2024 – June 2024  
Final report submitted: June 30, 2024. Due to overlap with established literature, the findings were not submitted for publication.

## Reflection and future direction
The relatively low statistical power, resulting from our small cohort size, limited our ability to perform meaningful analyses on all clinical and immunological variables initially collected. In future projects, I aim to work with larger cohorts, apply a multivariable modeling approach, and explore the implementation of machine learning techniques.
