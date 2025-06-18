# Enhancing-Patient-Triage
This project enhances Montanaro Hospital's OU efficiency. It uses data analytics and predictive models (Random Forest best) to identify factors (temp, BP, age, diagnosis) causing patient "flips" from observation to inpatient. The goal is to optimize patient triage and improve resource utilization.
Sure, here's a README for your GitHub project:

```markdown
# Enhancing Patient Triage Efficiency and Capacity in Montanaro Hospital's Observation Unit

## Project Overview

[cite_start]This project addresses key operational challenges within Montanaro Hospital's 23-bed Observation Unit (OU), specifically focusing on extended patient stays and the frequent transition of patients from observation to inpatient status ("flips")[cite: 1]. [cite_start]The primary goal is to enhance patient placement procedures to optimize care delivery and improve the efficient utilization of the Observation Unit[cite: 1, 2].

## Key Challenges

* [cite_start]**Extended Length of Stay:** Patients are staying longer than initially intended in the OU[cite: 3].
* [cite_start]**Observation to Inpatient Movement ("Flips"):** A significant number of patients are being transferred from observation to inpatient status[cite: 3].
* [cite_start]**Inefficient Utilization:** These challenges lead to inefficient use of the OU's capacity[cite: 3].

## Objectives

The project aims to:
* [cite_start]Identify key demographic and clinical factors contributing to patient "flips"[cite: 3].
* [cite_start]Develop predictive models to identify patients at high risk of flipping from observation to inpatient status[cite: 11].
* Provide data-driven recommendations for improving patient triage protocols and optimizing OU capacity.

## Methodology

### Data Description

[cite_start]The analysis utilized a dataset containing 1111 observations and 17 variables from Montanaro Hospital's OU[cite: 4]. Key variables include:
* [cite_start]`Age`: Age of Patient in Years[cite: 5].
* [cite_start]`Gender`: Patient Gender (Male/Female)[cite: 5].
* [cite_start]`Flipped`: Binary variable (1 – Patient Flipped, 0 – Patient stayed in OU)[cite: 5].
* [cite_start]`OU_LOS_hrs`: Length of stay in OU in Hours[cite: 5].
* [cite_start]`DRG01`: Initial Diagnosis related group[cite: 5].
* [cite_start]`BloodPressureLower` & `BloodPressureUpper`: Diastolic and Systolic blood pressure[cite: 5].
* [cite_start]`Temperature`: Patient temperature in Fahrenheit[cite: 5].
* [cite_start]`Temperature Category`: Categorized temperature (e.g., Below Normal, Normal, Fever)[cite: 5].
* [cite_start]`BP Category`: Categorized blood pressure (e.g., Normal, Elevated, Hypertension Stage 1)[cite: 5, 6, 7].

### Analysis and Modeling

1.  [cite_start]**Descriptive Analytics:** Explored the percentage of patients flipping from observation to inpatient status (53.9% of patients flipped)[cite: 5]. [cite_start]Analyzed flips by temperature category, primary diagnosis group (DRG01), blood pressure category, and age category[cite: 8, 9].
    * [cite_start]**Top Flipped Categories:** Normal Temperature (87.70% of flips), Prehypertension (48.83% of flips), and Age 81-90 (40.04% of flips) were significant contributors to patient flips[cite: 10].

2.  **Predictive Modeling:** Developed and evaluated three machine learning models:
    * [cite_start]**Logistic Regression** [cite: 11]
    * [cite_start]**Random Forest** [cite: 11]
    * [cite_start]**Decision Tree** [cite: 11]

## Model Performance

| Model              | Accuracy | AUC  | Sensitivity | Specificity |
| :----------------- | :------- | :--- | :---------- | :---------- |
| Logistic Regression| 0.76     | 0.84 | 0.70        | 0.82        |
| Random Forest      | 0.82     | 0.76 | 0.88        | 0.82        |
| Decision Tree      | 0.77     | 0.73 | 0.82        | [cite_start]0.78        [cite: 11]|

[cite_start]The **Random Forest** model demonstrated the highest accuracy (0.82) and sensitivity (0.88), making it the most effective for predicting patient flips and enabling proactive interventions[cite: 11].

## Recommendations

The project provides recommendations for improved operations, including:
* Implementing predictive analytics to aid triage decisions.
* Refining triage protocols for high-risk patient groups (e.g., based on age, blood pressure, specific diagnoses).
* [cite_start]Establishing continuous monitoring and feedback loops for protocol effectiveness[cite: 13].

```
