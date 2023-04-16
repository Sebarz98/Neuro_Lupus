# Neuro_Lupus
Investigating Systemic Lupus Erythematosus effects on volumetric brain MRI.

# Preliminary Analysis

## Feature Distribution 
### First 55 features

![feature_distribution](https://user-images.githubusercontent.com/70062910/232321176-20dc1a0c-c780-4c98-8231-575af1637d44.png)

### First 55 features with NP-SLE
For every feature distribution go to results/EDA then depending on the NP-EVENT, /Neuro or /Non_Neuro; for mean, median and sd go to 1, for percentiles and quantiles go to 2

![SLEDAI-2k (at the time of NP event)_distribution](https://user-images.githubusercontent.com/70062910/232322253-033d3533-b2c8-4cfe-9f15-f637aadfe004.png)
![C3 (mgdl)_distribution](https://user-images.githubusercontent.com/70062910/232322265-6238b3d0-a55b-412a-b52e-d5fe69034f36.png)
![Abnormal Appearing White Matter volume cm3_distribution](https://user-images.githubusercontent.com/70062910/232322282-583d9a37-2b6f-4545-b855-72c75a5798eb.png)
![Cortical Grey Matter volume cm3_distribution](https://user-images.githubusercontent.com/70062910/232322305-0d8a1595-b61f-4763-adc5-911954de8f8b.png)
![Cerebellar Grey Matter volume cm3_distribution](https://user-images.githubusercontent.com/70062910/232322318-5666f0de-773a-4567-8797-f62b195ed3f9.png)

### First 55 features without NP-SLE

![SLEDAI-2k (at the time of NP event)_distribution](https://user-images.githubusercontent.com/70062910/232322481-d306704f-44a2-498c-bd9c-70866fd4fd6a.png)
![C3 (mgdl)_distribution](https://user-images.githubusercontent.com/70062910/232322495-a56316bb-f8ce-4d7c-9635-1f27ea6752cb.png)
![Abnormal Appearing White Matter volume cm3_distribution](https://user-images.githubusercontent.com/70062910/232322502-4ab3d268-d327-4e98-8273-95cc553e6aa7.png)
![Cortical Grey Matter volume cm3_distribution](https://user-images.githubusercontent.com/70062910/232322507-280946dd-cf73-4945-9bb6-18b2069c2ac0.png)
![Cerebellar Grey Matter volume cm3_distribution](https://user-images.githubusercontent.com/70062910/232322512-878b1798-a312-4dc5-bc32-7548bbf862b5.png)

## Features Relationship
### Pair plot between SLEDAI (y-axis), prednisnone, anti-DNA and C3 (x-axis)

![pair_sledai_prednisnone_dsDNa_c3](https://user-images.githubusercontent.com/70062910/232322689-0abb5d7b-cd56-48ae-ba1f-b7d579376995.png)

### Strip plot between Disease Duration (y-axis) and various features

![stripplot_disease_dur_vs_continuous](https://user-images.githubusercontent.com/70062910/232322842-5a08fda3-ab05-4058-ae21-e0aff5afced1.png)
![stripplot_disease_dur_vs_features](https://user-images.githubusercontent.com/70062910/232322841-4356f17e-21b5-4b7d-8e23-d693221e7422.png)

### Violin plot between Disease Duration (y-axis) and various features

![violin_disease_against_features](https://user-images.githubusercontent.com/70062910/232322870-89e632fb-8cb5-4f0a-b973-2dc652cb6124.png)

### Correlation Matrix

![correlation_matrix](https://user-images.githubusercontent.com/70062910/232322890-351261b0-087c-4756-9b0a-6de50b2c7375.png)

Using NP-SLE as target column 

![correlation_target_event](https://user-images.githubusercontent.com/70062910/232322912-4f76704a-0c35-49c4-8029-82588342aeb3.png)

10 most correlated features with NP-SLE

![10_correlated_features](https://user-images.githubusercontent.com/70062910/232322932-66e715b7-114e-47c2-b9a0-067b9ad35a63.png)

## Descriptive Statistics

For the full descriptive statistics go to /code/Stats

<img width="563" alt="Screenshot 2023-04-16 at 17 39 17" src="https://user-images.githubusercontent.com/70062910/232324073-4d4076b8-ccd6-4423-a943-ee890f43cdc7.png">
<img width="639" alt="Screenshot 2023-04-16 at 17 39 35" src="https://user-images.githubusercontent.com/70062910/232324087-8ead1b4c-9b02-4b43-a4c3-58e2863b9a79.png">
<img width="413" alt="Screenshot 2023-04-16 at 17 39 58" src="https://user-images.githubusercontent.com/70062910/232324097-62f30a83-fa3f-43b3-8100-27b5ada7cf9b.png">

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

By groupying based on NP-SLE, clinical statistically significant variables were: ['aPL syndrome', 'AnAb ', 'Anti-Rib-P']

### Wilcoxon rank-sum test

Was conducted to compare continuous mri variables among groups based on NP-SLE 
Many were found to be statistically significant, the 5 most

![Wilcoxon](https://user-images.githubusercontent.com/70062910/232326022-b679f2b8-c470-4fa6-a115-c2f74bc7ad99.png)

### Fisher’s exact 

Was conducted to compare categorical variables among groups based on NP-SLE and AnAb
Odds ratio: 7.00; P-value: 0.0461

### Kruskal-Wallis test (equivalent of ANOVA)

<img width="666" alt="kruskal" src="https://user-images.githubusercontent.com/70062910/232326335-57229d36-097a-44e9-9b44-98924f0f86b1.png">

## Account for partial correlation

Neurocognitive z-scores of specific neuroclinical domains were correlated with Abnormal White Matteer across the subject groups using Pearson correlation. 
Adjusted for prednisone therapy (mg/day) and SLEDAI as partial correlations.

By adjusting with partial correlation no statistically significant correlation were found. 
