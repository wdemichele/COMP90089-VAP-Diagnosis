# COMP90089 Group Project

# Healthcare Acquired Infections (HAI) Analysis in MIMIC IV
# Phase 1

## Overview
In this project, we aim to analyze the MIMIC IV dataset to identify and explore patients with HAI (Healthcare Acquired Infections). This README provides a step-by-step guide of the processes involved, starting from data extraction to topic modeling.

## Table of Contents
1. Data Extraction
2. Data Pre-processing
3. Exploratory Data Analysis (EDA)
4. Topic Modeling using LDA
5. Conclusion

---

## 1. Data Extraction

### Objective:
To extract relevant data about patients with potential HAI from the MIMIC IV dataset using specific ICD codes.

### SQL Queries Used:
- Initial exploration of dataset to understand distribution of ICD codes.
- Extracted patients with relevant ICD codes indicating potential HAIs.
- Gathered associated clinical notes, demographics, lab results, pharmacy data, and procedures.

---

## 2. Data Pre-processing

### Objective:
To clean and transform the data to a format suitable for analysis.

### Steps:
- Managed missing values by either imputation or deletion, based on the nature of the data.
- Converted timestamp data to appropriate datetime format.
- Created relevant flags/indicators for specific conditions or events in the data.

---

## 3. Exploratory Data Analysis (EDA)

### Objective:
To gain insights into the dataset and understand patterns, especially around HAI.

### Steps:
- Descriptive statistics to understand central tendencies and distribution of data.
- Visualizations to see the distribution of age, gender, admission type, etc. among patients with HAI.
- Correlation analysis to understand the relationship between different variables.
- Identified outliers and examined their potential impact on the analysis.

---

## 4. Topic Modeling using LDA

### Objective:
To extract underlying topics from clinical notes to aid in confirming the presence of HAI.

### Steps:
- **Text Preprocessing:** 
  - Tokenized the clinical notes.
  - Removed stopwords and punctuation.
  - Lemmatized the words for standardization.
  
- **LDA Model Training:** 
  - Constructed a term-document matrix.
  - Trained the LDA model using Gensim.
  
- **Visualization:**
  - Used `pyLDAvis` for interactive visualization of topics.

---

## 5. Conclusion

The analysis provided insights into patients with potential HAI in the MIMIC IV dataset. By leveraging ICD codes, clinical notes, and various patient information, we aim to create a robust methodology for confirming HAI. The topic modeling using LDA offered insights into the main themes present in the clinical notes, aiding in the confirmation process.

We found that there is some useable information and traces of confirmation that HAI was prominent. With this NLP analysis we can use MIMIC iv Note to extract patient information for more in depth analysis using specific lab test results to further refine for the creation of the "Risk" factor for HAI of a patient cohort.

--- 
