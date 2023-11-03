# Diagnosing Ventilator-Associated Pneumonia: A Machine Learning Approach with MIMIC-IV Data
COMP90089 - Group 3, Semester 2, 2023
- William De Michele
- Mohit Rudraraju Suresh
- Azmi
- Chinatip Kultanapanit
- Hanyu Wang

## Objective
Improves VAP diagnosis by optimizing ML models for early identification and management

## Notebooks
### Data exploration & Data Extraction
Explore data related to Central Line-Associated Bloodstream Infections (CLABSIs), Catheter-Associated Urinary Tract Infections (CAUTIs), Ventilator Associated Pneumonia (VAP) on MIMIC-IV database
- [ML_Health_NLP_explore](https://github.com/wdemichele/COMP90089-Group-Project/blob/main/ML_Health_NLP_explore%20.ipynb) - Discover patients with HAIs (CAUTI, CLABSI, VAP) using ICD codes and NLP
- [Recent_Surgery](https://github.com/wdemichele/COMP90089-Group-Project/blob/main/Recent_Surgery.ipynb) - Surgery records related to with HAIs (CAUTI, CLABSI, VAP)
- [Vital_Signs](https://github.com/wdemichele/COMP90089-Group-Project/blob/main/Vital_Signs.ipynb) - Statistical data on vital signs related to HAI-positive patients
- [ventilation](https://github.com/wdemichele/COMP90089-Group-Project/blob/main/ventilation.ipynb) - Records of treatments involving invasive devices
- [HAI_Basic_Info](https://github.com/wdemichele/COMP90089-Group-Project/blob/main/HAI_Basic_Info.ipynb) - Basic infomation could related to HAIs
- [Extract_Patients](https://github.com/wdemichele/COMP90089-Group-Project/blob/main/Extract_Patients.ipynb) - Extract HAI positive patients (VAP)
### Data processing
End-to-End Data Processing with Data Preprocessing, Model Building, and Model Evaluation
- [HAI_Supervised_Learning](https://github.com/wdemichele/COMP90089-Group-Project/blob/main/HAI_Supervised_Learning.ipynb) - Neural Model
    - Handles complex structured data, optimized parameters using grid search, and utilizes adaptive learning rates with Adam optimizer
- [HAI_Supervised_Learning_Classical](https://github.com/wdemichele/COMP90089-Group-Project/blob/main/HAI_Supervised_Learning_Classical.ipynb) - Classical Model (Naive Bayes, SVM, RFC)
    - Naives Bayes: Simplicity & Simplicity, but limited ability to capture complex relationships
    - Random Forest Classifier (RFC): Better handling of interdependencies, but underperformed in recall for the VAP Positive class
### Data
Collected from MIMIC-IV databases
- [patient_cohort_features_vap](https://github.com/wdemichele/COMP90089-Group-Project/blob/main/patient_cohort_features_vap.zip) - A cohort of patients with Ventilator-Associated Pneumonia (VAP) was identified from the MIMIC database using a combination of ICD codes and Natural Language Processing (NLP) techniques.
    - Compute statistical summaries for numeric features (mean, Q1, Q2, Q3, standard deviation, variance, min, max) to capture feature distributions
    - Analyze patient vital signs, measuring duration and episodes above/below normal conditions
    - Calculate ventilator duration, capturing the time between start and stop procedure times

## Resources
MIMIC-IV docs: [link](https://mimic.mit.edu/docs/iv/)