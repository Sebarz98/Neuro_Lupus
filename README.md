# Neuro_Lupus
Investigating Systemic Lupus Erythematosus effects on volumetric brain MRI.

# Preliminary Analysis

#### Distributions were checked for normality and homogenity
#### Statistical significance has been evaluated for a p-value < 0.05

### Welch T-test

By groupying based on NP-SLE, clinical statistically significant variables were:['aPL syndrome', 'AnAb ', 'Anti-Rib-P']

### Wilcoxon rank-sum test

Was conducted to compare continuous mri variables among groups based on NP-SLE 
Many were found to be statistically significant, the 5 most were: CO Total volume %, OCP total thickness norm,  OCP left thickness norm,  Ang right thickness mm,  OCP total thickness mm. <br />

For SLEDAI (< or > 4): Ent left volume cm3, Ent total volume %, Ent total volume cm3, Gray Matter volume %, PT right thickness norm <br />

For dsDNA titre: CO right volume %, Insula right volume %, OpIFG thickness asymmetry, Brainstem volume %, FuG thickness asymmetry <br />

For Anti-Ro-SSA: Frontal volume asymmetry, GRe volume asymmetry, MOG right volume cm3, OrIFG left volume %, MOG right volume % <br />

For Anti-RNP: FuG left volume %, FuG total volume %, FuG total volume cm3, FuG left volume cm3, FuG right volume % <br />

For LAC: OFuG left thickness norm, OFuG total thickness norm, Cerebellum WM total volume %, Cerebellum WM right volume %, OFuG left thickness mm <br />

For Anti-Sm: LiG volume asimmetry, LiG left volume %, PCgG right thickness norm, FO volume asymmetry, PCgG right thickness mm <br /> 

For aPL: PHG volume asimmetry, TTG thickness asimmetry, Thalamus volume asimmetry, Temporal total volume %, Temporal right volume % <br />

For AnAb: AnG right thickness mm, OrIFG right thickness mm, CO volume asymmetry, OrIFG right thickness norm, SCA left thickness mm <br />

For Anti-Rib-P: AnG right thickness mm, OpIFG left volume cm3, Cerebellar Gray Matter volume cm3, Cerebellar Gray Matter right volume cm3, Cerebellar Gray Matter total volume cm3 <br />

For Anti-DWEYS: Cerebellar Vermal Lobule VII volume cm3, LiG left volume cm3, OCP left volume cm3, OCP total volume cm3, MPrG right volume % <br />

For Cutaneous Vasculitis:  AnG right volume cm3,  AnG left volume cm3, MPrG left volume %, PT left thickness mm, iOG left volume cm3 <br />

For Hypertension: OpIFG right volume %, OpIFG left volume %, TTG total thickness mm, TG total thickness norm, AnG right volume % <br />

For smoking: PHG left volume cm3, PT right thickness mm, STG volume asymmetry, Cerebrum GM volume asymmetry, OrIFG thickness asymmetry <br />


### Fisher’s exact 

Was conducted to compare categorical variables among groups, based on NP-SLE and AnAb:
Odds ratio: 7.00; P-value: 0.0461

Was conducted to compare categorical variables among groups, based on NP-SLE and Anti-Rib-P:
Odds ratio: 9.00; P-value: 0.0768

## Correlation Analysis

### Correlation Matrix

![correlation_matrix](https://user-images.githubusercontent.com/70062910/232322890-351261b0-087c-4756-9b0a-6de50b2c7375.png)

Using NP-SLE as target column 

![correlation_target_event](https://user-images.githubusercontent.com/70062910/232322912-4f76704a-0c35-49c4-8029-82588342aeb3.png)

10 most correlated features with NP-SLE

![10_correlated_features](https://user-images.githubusercontent.com/70062910/232322932-66e715b7-114e-47c2-b9a0-067b9ad35a63.png)

### Correlation Coefficients

Spearman Correlation Coefficient was calculated for the features that did not met normality assumptions

For Disease duration (months): <br />
FuG volume asymmetry                         0.797314 <br />
PT thickness asymmetry                       0.527473 <br />
Hypertension                                 0.462805 <br />

For SLEDAI-2k (at the time of NP event): <br />
PIns thickness asymmetry                               0.290418 <br />
MPrG right thickness mm                                0.238174 <br />
Hypertension                                           0.228016 <br />

For PGA (at the time of fMRI): <br />
PT thickness asymmetry                       0.278617 <br />
PO total thickness mm                        0.260513 <br />
PCgG left volume %                           0.239647 <br />

For SLICC-DI (at the time of NP event): <br />
ever smoking                                          0.456071 <br />
PT right thickness norm.                              0.450192 <br />
PT right thickness mm                                 0.448960 <br />


### Partial Correlation

Neurocognitive z-scores of specific neuroclinical domains were correlated with Abnormal White Matteer across the subject groups using Pearson correlation. 
Adjusted for prednisone therapy (mg/day) and SLEDAI as partial correlations.

By adjusting with partial correlation no statistically significant correlation were found. 

Other Correlation with neuro events and NP-SLE (as result). The top 5 correlated features with NP-SLE were tested.

total_neurocog vs SCA thickness asymmetry: r = 0.51, p = 0.01 <br />
result vs SCA thickness asymmetry (partial corr): r = 0.34, p = 0.09 <br />
Event_Seizure, ACS, myelitis, CVA vs SCA thickness asymmetry: r = 0.20, p = 0.31 <br />
Event_Seizure, ACS, myelitis, CVA vs SCA thickness asymmetry (partial corr): r = 0.39, p = 0.06 <br />

total_neurocog vs Amygdala right volume %: r = 0.46, p = 0.02 <br />
result vs Amygdala right volume % (partial corr): r = 0.39, p = 0.05 <br />
Event_Seizure, ACS, myelitis, CVA vs Amygdala right volume %: r = 0.13, p = 0.53 <br />
Event_Seizure, ACS, myelitis, CVA vs Amygdala right volume % (partial corr): r = 0.14, p = 0.51 <br />

total_neurocog vs Temporal thickness asymmetry: r = 0.44, p = 0.02 <br />
result vs Temporal thickness asymmetry (partial corr): r = 0.48, p = 0.02 <br />
Event_Seizure, ACS, myelitis, CVA vs Temporal thickness asymmetry: r = 0.45, p = 0.02 <br />
Event_Seizure, ACS, myelitis, CVA vs Temporal thickness asymmetry (partial corr): r = 0.57, p = 0.00 <br />

total_neurocog vs TMP thickness asymmetry: r = 0.43, p = 0.03 <br />
result vs TMP thickness asymmetry (partial corr): r = 0.44, p = 0.03 <br />
Event_Seizure, ACS, myelitis, CVA vs TMP thickness asymmetry: r = 0.73, p = 0.00 <br />
Event_Seizure, ACS, myelitis, CVA vs TMP thickness asymmetry (partial corr): r = 0.84, p = 0.00 <br />

total_neurocog vs MTG thickness asymmetry: r = 0.43, p = 0.03 <br />
result vs MTG thickness asymmetry (partial corr): r = 0.47, p = 0.02 <br />
Event_Seizure, ACS, myelitis, CVA vs MTG thickness asymmetry: r = 0.41, p = 0.03 <br />
Event_Seizure, ACS, myelitis, CVA vs MTG thickness asymmetry (partial corr): r = 0.48, p = 0.02 <br />

### SLEDAI <br />

Event_Seizure, ACS, myelitis, CVA vs SLEDAI-2k (at the time of NP event): r = 0.30, p = 0.12 <br />
Event_Seizure, ACS, myelitis, CVA vs SLEDAI-2k (at the time of NP event) (partial corr): r = 0.64, p = 0.00 <br /> 
IOG volume asymmetry vs SLEDAI-2k (at the time of NP event): r = 0.42, p = 0.03 <br />
IOG volume asymmetry vs SLEDAI-2k (at the time of NP event) (partial corr): r = 0.55, p = 0.00 <br />
Event_CVA vs IOG volume asymmetry: r = -0.28, p = 0.16 <br />
Event_CVA vs IOG volume asymmetry (partial corr): r = -0.34, p = 0.10 <br />
Event_Mood abnormalities (depressive) vs IOG volume asymmetry: r = 0.23, p = 0.24 <br />
Event_Mood abnormalities (depressive) vs IOG volume asymmetry (partial corr): r = 0.07, p = 0.73 <br />
Event_Mood abnormalities (mixed) vs IOG volume asymmetry: r = 0.30, p = 0.13 <br /> 
Event_Mood abnormalities (mixed) vs IOG volume asymmetry (partial corr): r = 0.33, p = 0.10 <br />

Calc total volume % vs SLEDAI-2k (at the time of NP event): r = 0.39, p = 0.04 <br />
Calc total volume % vs SLEDAI-2k (at the time of NP event) (partial corr): r = 0.48, p = 0.02 <br />
Event_Seizure vs Calc total volume %: r = -0.47, p = 0.01 <br />
Event_Seizure vs Calc total volume % (partial corr): r = -0.33, p = 0.11 <br />

Amygdala total volume % vs SLEDAI-2k (at the time of NP event): r = 0.38, p = 0.05 <br />
Amygdala total volume  % vs SLEDAI-2k (at the time of NP event) (partial corr): r = 0.21, p = 0.31 <br />
Event_Movement Disorder vs Amygdala total volume %: r = 0.30, p = 0.13 <br />
Event_Movement Disorder vs Amygdala total volume % (partial corr): r = 0.27, p = 0.20 <br />

Event_CVA vs PHG total thickness norm.: r = -0.30, p = 0.13 <br />
Event_CVA vs PHG total thickness norm. (partial corr): r = -0.51, p = 0.01 <br />

4th Ventricle volume % vs SLEDAI-2k (at the time of NP event): r = 0.32, p = 0.10 <br />
4th Ventricle volume % vs SLEDAI-2k (at the time of NP event) (partial corr): r = 0.45, p = 0.03 <br />
Event_Seizure, ACS, myelitis, CVA vs 4th Ventricle volume %: r = 0.33, p = 0.10 <br />
Event_Seizure, ACS, myelitis, CVA vs 4th Ventricle volume % (partial corr): r = 0.52, p = 0.01 <br />

### SLICC <br />

Event_Mood abnormalities (depressive) vs SLICC-DI (at the time of NP event): r = -0.15, p = 0.45 <br />
Event_Mood abnormalities (depressive) vs SLICC-DI (at the time of NP event) (partial corr): r = -0.42, p = 0.04 <br /> 
Event_Psychosis vs SLICC-DI (at the time of NP event): r = 0.45, p = 0.02<br /> 
Event_Psychosis vs SLICC-DI (at the time of NP event) (partial corr): r = 0.64, p = 0.00 <br />

OpIFG total volume % vs SLICC-DI (at the time of NP event): r = -0.61, p = 0.00 <br />
OpIFG total volume % vs SLICC-DI (at the time of NP event) (partial corr): r = -0.49, p = 0.01 <br /> 

MPoG right volume % vs SLICC-DI (at the time of NP event): r = -0.54, p = 0.00 <br />
MPoG right volume % vs SLICC-DI (at the time of NP event) (partial corr): r = -0.37, p = 0.07 <br />

Ventral DC left volume % vs SLICC-DI (at the time of NP event): r = -0.49, p = 0.01 <br />
Ventral DC left volume % vs SLICC-DI (at the time of NP event) (partial corr): r = -0.56, p = 0.0 <br />

Event_Mood abnormalities (mixed) vs Ventral DC left volume %: r = 0.33, p = 0.10 <br />
Event_Mood abnormalities (mixed) vs Ventral DC left volume % (partial corr): r = 0.39, p = 0.06 <br />

Insular right thickness mm vs SLICC-DI (at the time of NP event): r = -0.49, p = 0.01 <br />
Insular right thickness mm vs SLICC-DI (at the time of NP event) (partial corr): r = -0.42, p = 0.03 <br />

Event_Mood abnormalities (depressive) vs Insular right thickness mm: r = 0.29, p = 0.14 <br />
Event_Mood abnormalities (depressive) vs Insular right thickness mm (partial corr): r = 0.40, p = 0.05 <br />

MG total volume % vs SLICC-DI (at the time of NP event): r = -0.51, p = 0.01 <br />
SMG total volume % vs SLICC-DI (at the time of NP event) (partial corr): r = -0.43, p = 0.03 <br />

Event_CVA vs SMG total volume %: r = -0.33, p = 0.10 <br />
Event_CVA vs SMG total volume % (partial corr): r = -0.42, p = 0.03 <br />

### dsDNA  <br />

Event_Seizure vs anti-dsDNA Titre  (insert NV here <7 ): r = 0.12, p = 0.55 <br />
Event_Seizure vs anti-dsDNA Titre  (insert NV here <7 ) (partial corr): r = 0.56, p = 0.00 <br />

AOrG thickness asymmetry vs anti-dsDNA Titre  (insert NV here <7 ): r = -0.47, p = 0.01 <br />
AOrG thickness asymmetry vs anti-dsDNA Titre  (insert NV here <7 ) (partial corr): r = -0.23, p = 0.27 <br />
Event_Seizure, ACS, myelitis, CVA vs AOrG thickness asymmetry: r = -0.28, p = 0.16 <br />
Event_Seizure, ACS, myelitis, CVA vs AOrG thickness asymmetry (partial corr): r = -0.38, p = 0.06 <br />

SPL volume asymmetry vs anti-dsDNA Titre  (insert NV here <7 ): r = -0.43, p = 0.03 <br />
SPL volume asymmetry vs anti-dsDNA Titre  (insert NV here <7 ) (partial corr): r = -0.01, p = 0.96 <br />

AnG total thickness mm vs anti-dsDNA Titre  (insert NV here <7 ): r = -0.43, p = 0.03 <br />
AnG total thickness mm vs anti-dsDNA Titre  (insert NV here <7 ) (partial corr): r = -0.25, p = 0.23 <br />

Event_Seizure, ACS, myelitis, CVA vs AnG total thickness mm: r = -0.33, p = 0.10 <br />
Event_Seizure, ACS, myelitis, CVA vs AnG total thickness mm (partial corr): r = -0.47, p = 0.02 <br />

AnG left thickness mm vs anti-dsDNA Titre  (insert NV here <7 ): r = -0.41, p = 0.04 <br />
AnG left thickness mm vs anti-dsDNA Titre  (insert NV here <7 ) (partial corr): r = -0.37, p = 0.07 <br />

Event_Seizure vs AnG left thickness mm: r = -0.48, p = 0.01 <br />
Event_Seizure vs AnG left thickness mm (partial corr): r = -0.24, p = 0.24 <br />
Event_Seizure, ACS, myelitis, CVA vs AnG left thickness mm: r = -0.33, p = 0.10 <br />
Event_Seizure, ACS, myelitis, CVA vs AnG left thickness mm (partial corr): r = -0.38, p = 0.06 <br />

### C3 mg/dL <br />

Event_Mood abnormalities (mixed) vs C3 (mgdl): r = 0.28, p = 0.16 <br />
Event_Mood abnormalities (mixed) vs C3 (mgdl) (partial corr): r = 0.40, p = 0.04 <br />

Event_Movement Disorder vs AnG left thickness mm: r = 0.30, p = 0.13 <br />
Event_Movement Disorder vs AnG left thickness mm (partial corr): r = 0.35, p = 0.09 <br />
Event_Seizure vs AnG left thickness mm: r = -0.48, p = 0.01 <br />
Event_Seizure vs AnG left thickness mm (partial corr): r = -0.24, p = 0.24 <br />
Event_Seizure, ACS, myelitis, CVA vs AnG left thickness mm: r = -0.33, p = 0.10 <br />
Event_Seizure, ACS, myelitis, CVA vs AnG left thickness mm (partial corr): r = -0.38, p = 0.06 <br />

Calc right volume cm3 vs C3 (mgdl): r = -0.56, p = 0.00 <br />
Calc right volume cm3 vs C3 (mgdl) (partial corr): r = -0.56, p = 0.00 <br />

Event_Seizure vs Calc right volume cm3: r = -0.41, p = 0.03 <br />
Event_Seizure vs Calc right volume cm3 (partial corr): r = -0.16, p = 0.44 <br />

Event_CVA vs Calc right volume cm3: r = -0.33, p = 0.10 <br />
Event_CVA vs Calc right volume cm3 (partial corr): r = -0.35, p = 0.09 <br />

PCu right thickness mm vs C3 (mgdl): r = 0.52, p = 0.01 <br />
PCu right thickness mm vs C3 (mgdl) (partial corr): r = 0.46, p = 0.02 <br />

Event_Seizure, ACS, myelitis, CVA vs PCu right thickness mm: r = -0.33, p = 0.10 <br />
Event_Seizure, ACS, myelitis, CVA vs PCu right thickness mm (partial corr): r = -0.45, p = 0.02 <br />

MOG volume asymmetry vs C3 (mgdl): r = 0.48, p = 0.01 <br />
MOG volume asymmetry vs C3 (mgdl) (partial corr): r = 0.37, p = 0.07 <br />

### C4 mg/dL <br />

MTG volume asymmetry vs C4 (mgdl): r = 0.54, p = 0.00 <br />
MTG volume asymmetry vs C4 (mgdl) (partial corr): r = 0.52, p = 0.01 <br />

PIns total volume cm3 vs C4 (mgdl): r = 0.54, p = 0.00 <br />
PIns total volume cm3 vs C4 (mgdl) (partial corr): r = 0.47, p = 0.02 <br />

FRP right volume cm3 vs C4 (mgdl): r = 0.55, p = 0.00 <br />
FRP right volume cm3 vs C4 (mgdl) (partial corr): r = 0.39, p = 0.06 <br />
Event_Seizure vs FRP right volume cm3: r = 0.42, p = 0.03 <br />
Event_Seizure vs FRP right volume cm3 (partial corr): r = 0.48, p = 0.01 <br />

ITG thickness asymmetry vs C4 (mgdl): r = 0.67, p = 0.00 <br />
ITG thickness asymmetry vs C4 (mgdl) (partial corr): r = 0.56, p = 0.00 <br />

## Regression Analysis <br />

### Ordinary Least Square Regression <br />

With 10 most correlated variables <br />

#### SLEDAI as target  <br />
R-Squared: 0.725 <br />
Adj. R-Squared 0.553 <br />

#### SLICC as target  <br />
R-Squared: 0.715 <br />
Adj. R-Squared 0.537 <br />

#### dsDNA as target  <br />
R-Squared: 0.234 <br />
Adj. R-Squared - 0.245 <br />

#### C3 mg/dL as target  <br />
R-Squared: 0.622 <br />
Adj. R-Squared 0.386 <br />

#### PGA as target  <br />
R-Squared: 0.662 <br />
Adj. R-Squared 0.451 <br />

## Random Forest Model

3 random forest models were deployed to differentiate between non NP-SLE and NP-SLE. <br />
The best one used Boruta for feature selection. <br />

Random Forest accuracy:  83.33 % <br />

1. The F-1 Score of the model: 0.83 <br />

2. The Recall Score of the model: 0.83 <br />

3. Classification report: <br />
              precision    recall  f1-score   support

           0       0.75      1.00      0.86         3
           1       1.00      0.67      0.80         3

    accuracy                           0.83         6
   macro avg       0.88      0.83      0.83         6
weighted avg       0.88      0.83      0.83         6


4. AUC: 0.8333333333333333 <br />
Specificity (TNR): 1.0 <br />
Precision (PPV): 1.0 <br />
Negative Predictive Value (NPV): 0.75 <br />
False Positive Rate (FPR): 0.0 <br />
