# Neuro_Lupus
Investigating Systemic Lupus Erythematosus effects on volumetric brain MRI.

# Preliminary Analysis

#### Distributions were checked for normality and homogenity
#### Statistical significance has been evaluated for a p-value < 0.05

## Parametric Tests

### T-Test
T-Test between NP-SLE and not was conducted amongst mri features, as normally distributed. 
Amidst the statistically relevant regions found: 'Amygdala total volume %', OpIFG total volume cm3', 'MFC left volume %', 'SMC volume asymmetry', 'Occipital left volume cm3','SOG total thickness mm', 'OCP left thickness norm.', 'AIns thickness asymmetry'. 

#### Cat plot with Abnormal White matter on y-axis, NP-SLE on x-axis and Disease Duration as other grouping

![T_test_white_duration_NP](https://user-images.githubusercontent.com/70062910/232325116-894bf5d4-3d41-4bfa-9969-1530182d022b.png)

#### Cat plot with Abnormal White matter on y-axis, AnAb on x-axis and Disease Duration as other grouping

![T_test_white_duration_AnAb](https://user-images.githubusercontent.com/70062910/232325132-2f7738ca-78b9-4fc6-81e0-a24a31519fdf.png)

#### Cat plot with Abnormal White matter on y-axis, aPL on x-axis and Disease Duration as other grouping

![T_test_white_duration_aPL](https://user-images.githubusercontent.com/70062910/232325149-4bf26ce9-7e2f-4be5-b8fe-525ee80fdcf8.png)

#### Pair gird plot with Abnormal White matter on y-axis, aPL on x-axis and NP-SLE as other grouping

![T_test_white_aPL_NP](https://user-images.githubusercontent.com/70062910/232325229-56f848fd-3add-4689-b6d7-2519c8de1c1b.png)

#### Pair gird plot with Abnormal White matter on y-axis, AnAb on x-axis and NP-SLE as other grouping

![T_test_white_AnAb_NP](https://user-images.githubusercontent.com/70062910/232325246-87f0e843-e6b8-4277-aa00-f552c58534ee.png)

### One-way analysis of variance (ANOVA) with F-Distribution

H0 not rejected for Abnormal White Matter based on NP-SLE
![F_dist_NP_White](https://user-images.githubusercontent.com/70062910/232325830-2e63c86d-b221-4348-bbf2-73e26fcb024e.png)

H0  rejected for SCA Thickness asymmetry based on NP-SLE
![F_dist_NP_SCA](https://user-images.githubusercontent.com/70062910/232325837-85a50f56-6db7-43a6-b714-968277fa619a.png)

### Chi-Square

Chi-Square test was conducted on AnAb and aPL, but was not statistically significant

## Non Parametric Tests

### Welch T-test

By groupying based on NP-SLE, clinical statistically significant variables were:['aPL syndrome', 'AnAb ', 'Anti-Rib-P']

### Wilcoxon rank-sum test

Was conducted to compare continuous mri variables among groups based on NP-SLE 
Many were found to be statistically significant, the 5 most were plotted.

![Wilcoxon](https://user-images.githubusercontent.com/70062910/232326022-b679f2b8-c470-4fa6-a115-c2f74bc7ad99.png)

### Fisher’s exact 

Was conducted to compare categorical variables among groups based on NP-SLE and AnAb:
Odds ratio: 7.00; P-value: 0.0461

### Kruskal-Wallis test (equivalent of ANOVA)

<img width="666" alt="kruskal" src="https://user-images.githubusercontent.com/70062910/232326335-57229d36-097a-44e9-9b44-98924f0f86b1.png">

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

## Regression Analysis

A linear regression was employed by using: 

target = 'NP-SLE' <br />

predictors = ['SCA thickness asymmetry', 'Amygdala right volume %', 'Temporal thickness asymmetry', 'TMP thickness asymmetry', 'MTG thickness asymmetry', 'AnAb ', 'aPL syndrome'] <br />

Mean Squared Error:  0.29831871364555906 <br />
R-squared:  -1.1478947382480253 <br />

Not significant. 

A logistic regression was attempted. <br />
Logistic Regression's accuracy:  66.67 % <br />
The F-1 Score of the model: 0.4 <br />
The Recall Score of the model: 0.4 <br />
AUC:0.4 <br />
Sensitivity (TPR): 0.8 <br />
Specificity (TNR): 0.0 <br />
Precision (PPV): 0.8 <br />
Negative Predictive Value (NPV): 0.0 <br />
False Positive Rate (FPR): 1.0 <br />

## Random Forest Model

3 random forest models were deployed. <br />
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
