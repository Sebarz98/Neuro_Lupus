# Neuro_Lupus
Investigating Systemic Lupus Erythematosus effects on volumetric brain MRI.

# Preliminary Analysis

## Feature Distribution 
###First 55 features

![feature_distribution](https://user-images.githubusercontent.com/70062910/232321176-20dc1a0c-c780-4c98-8231-575af1637d44.png)

###First 55 features with NP-SLE
For every feature descriptive statistics go to /code/Stats

![SLEDAI-2k (at the time of NP event)_distribution](https://user-images.githubusercontent.com/70062910/232322253-033d3533-b2c8-4cfe-9f15-f637aadfe004.png)
![C3 (mgdl)_distribution](https://user-images.githubusercontent.com/70062910/232322265-6238b3d0-a55b-412a-b52e-d5fe69034f36.png)
![Abnormal Appearing White Matter volume cm3_distribution](https://user-images.githubusercontent.com/70062910/232322282-583d9a37-2b6f-4545-b855-72c75a5798eb.png)
![Cortical Grey Matter volume cm3_distribution](https://user-images.githubusercontent.com/70062910/232322305-0d8a1595-b61f-4763-adc5-911954de8f8b.png)
![Cerebellar Grey Matter volume cm3_distribution](https://user-images.githubusercontent.com/70062910/232322318-5666f0de-773a-4567-8797-f62b195ed3f9.png)

###First 55 features without NP-SLE

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



