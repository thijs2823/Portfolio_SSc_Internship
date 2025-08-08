| Variable Name             | Type           | Values / Categories                                           | Description                                               |
|---------------------------|----------------|----------------------------------------------------------------|-----------------------------------------------------------|
| VISIT                     | Factor         | Baseline visit, Follow-up                                     | Patient visit time point: baseline or follow-up           |
| VISITNUM                  | Factor         | Follow-Up - 0, Follow-Up - 1, Follow-Up - 2, etc.              | Visit occasion (Follow-Up - 0 is at baseline)             |
| VSDTC                     | Date           | YYYY-MM-DD                                                    | Date of Visit                                             |
| VISITDY                   | Numeric        | Integer                                                       | Day number of visit relative to the baseline              |
| ASTDT_years               | Numeric        | Float                                                         | Years relative to the baseline                            |
| CEOCCUR                   | Numeric/Binary | 0 = no progression, 1 = progression                           | Indicator whether disease progression occurred            |
| CNSR                      | Numeric/Binary | 0 = censored (no event), 1 = event                            | Survival analysis censoring/event indicator               |
| SEX                       | Numeric/Binary | 0 = Male, 1 = Female                                          | Patient sex                                               |
| AGE                       | Numeric        | Years                                                         | Age of patient at visit                                   |
| SMOKE                     | Numeric/Binary | 1 = ever smoked, 0 = never smoked                             | Smoking status - ever smoked or not                       |
| SMOKING                   | Numeric/Binary | 1 = current smoker, 0 = non-smoker                            | Smoking status at the time of visit                       |
| LBTEST_ESR                | Numeric        | mm/hour                                                       | Erythrocyte sedimentation rate (ESR) in mm/hour           |
| LBTEST_CAPDEN             | Numeric        | Capillaries per millimeter                                    | Capillary density measured via nailfold capillaroscopy    |
| RPYN                      | Numeric/Binary | 1 = positive, 0 = negative                                    | Presence of Raynaud’s phenomenon                          |
| RPDUR                     | Numeric        | Months                                                        | Duration of Raynaud’s phenomenon in months                |
| PUFFYFING                 | Numeric/Binary | 1 = positive, 0 = negative                                    | Presence of ‘puffy fingers’                               |
| PUFFYDUR                  | Numeric        | Months                                                        | Duration of puffy fingers in months                       |
| LBTEST_ANA                | Numeric/Binary | 1 = positive, 0 = negative                                    | ANA (antinuclear antibodies) status                       |
| LBTEST_ENA                | Numeric/Binary | 1 = positive, 0 = negative                                    | ENA antibody status                                       |
| LBTEST_ACA                | Numeric/Binary | 1 = positive, 0 = negative                                    | Anti-centromere antibody (ACA) status                     |
| LBTEST_ATA                | Numeric/Binary | 1 = positive, 0 = negative                                    | Anti-topoisomerase antibody (ATA) status                  |
| LBTEST_ARA                | Numeric/Binary | 1 = positive, 0 = negative                                    | Anti-RNA polymerase III antibody (ARA) status             |
| LBTEST_AntiFibrillarin    | Numeric/Binary | 1 = positive, 0 = negative                                    | AntiFibrillarin status                                    |
| LBTEST_AntiNOR90          | Numeric/Binary | 1 = positive, 0 = negative                                    | AntiNOR90 status                                          |
| LBTEST_AntiPMScl          | Numeric/Binary | 1 = positive, 0 = negative                                    | AntiPMScl status                                          |
| LBTEST_AntiKu             | Numeric/Binary | 1 = positive, 0 = negative                                    | AntiKu status                                             |
| LBTEST_AntiPDGFR          | Numeric/Binary | 1 = positive, 0 = negative                                    | AntiPDGFR status                                          |
| LBTEST_AntiSSARo          | Numeric/Binary | 1 = positive, 0 = negative                                    | AntiSSARo status                                          |
| LBTEST_Antihiston         | Numeric/Binary | 1 = positive, 0 = negative                                    | Antihiston status                                         |
| LBTEST_AntiJo1            | Numeric/Binary | 1 = positive, 0 = negative                                    | AntiJo1 status                                            |
| LBTEST_AntiSM             | Numeric/Binary | 1 = positive, 0 = negative                                    | AntiSM status                                             |
| LBTEST_AntiRNP            | Numeric/Binary | 1 = positive, 0 = negative                                    | AntiRNP status                                            |
| LBTEST_AntiribosomaalP    | Numeric/Binary | 1 = positive, 0 = negative                                    | AntiribosomaalP status                                    |
| ENA_GRP                   | Factor         | ENA_negative, ENA_ACA, ENA_ATA, ENA_other                     | ENA autoantibody groups used in survival analyses         |
| CLVAL                     | Numeric/Binary | 1 = positive, 0 = negative                                    | Presence of telangiectasia                               |
| LBTEST4                   | Factor         | 1 = ≤ 7, 2 = >7                                               | Categorization of mean capillary density                  |
| AGEGR3                    | Factor         | 3 groups: 20-45, 45-60, 60+ years                             | Age group categories                                      |
| TELANG                    | Factor         | 1 = positive, 0 = negative                                    | Telangiectasia status                                     |
| CAPDENS7                  | Factor         | 1 or 2 (≤7 vs >7)                                             | Capillary density category                                |
| NCM_SCLERPAT              | Factor         | Early, Active, Late, None                                     | Scleroderma pattern detected by nailfold capillaroscopy   |
