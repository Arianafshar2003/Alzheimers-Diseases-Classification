# 🧠 Alzheimer’s Diseases Classification
### Machine Learning Final Project  
**Student:** Arian Afshar  
**Instructor:** Dr. Baghdadi  
**University:** Amirkabir University of Technology (Tehran Polytechnic)

---

## Table of Contents

1. [Project Overview](#project-overview)  
2. [Dataset](#dataset)  
3. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)  
4. [Data Preprocessing](#data-preprocessing)  
5. [Feature Selection](#feature-selection)  
6. [Modeling & Evaluation](#modeling--evaluation)  
7. [Results & Insights](#results--insights)  
8. [Presentation](#presentation)  
9. [How to Run](#how-to-run)  
10. [Acknowledgements](#acknowledgements)  
11. [License](#license)  
12. [توضیحات فارسی برای دانشجویان و اساتید ایرانی](#توضیحات-فارسی-برای-دانشجویان-و-اساتید-ایرانی)

---

## Project Overview

This project aims to classify **Alzheimer’s Disease** patients using clinical, lifestyle, and demographic data.  
Built as a complete data science pipeline for the *Machine Learning* course, it covers every stage: EDA, preprocessing, feature selection, modeling, evaluation, and conclusion—mirrored in the presentation slides.

---

## Dataset

- **Source:** Kaggle Alzheimer’s Diseases (public dataset)
- **Size:** 429 samples, 35 features
- **Features:** Age, Gender, Education, BMI, Medical history (e.g., Diabetes, Hypertension), Lab values, Cognitive scores, etc.
- **Target variable:** Diagnosis (classification label)
- **Missing Data:** No missing values detected (clean dataset)
- **Note:** Imputation and preprocessing steps are shown for completeness

---

## Exploratory Data Analysis (EDA)

- **Data Types:**  
  - *Numerical features:* (Age, BMI, Lab values, MMSE, Functional scores, etc.)
  - *Categorical features:* (Gender, EducationLevel, Smoking, FamilyHistory, etc.)
- **Distributions:**  
  - Age is centered around 90, typical for Alzheimer’s cohorts
  - Some features are balanced, others (e.g. Gender, Family History) imbalanced
- **Target Analysis:**  
  - Diagnosis classes visualized
- **Visualizations + Tables:**  
  - Histograms, value counts for core features

---

## Data Preprocessing

- **Categorical variable encoding**  
- **Outlier detection & removal**  
- **Class balancing:** Applied [SMOTE](https://imbalanced-learn.org/stable/references/generated/imblearn.over_sampling.SMOTE.html)  
- **Training/Test splitting**
- **Scaling:** Normalization & Standardization

---

## Feature Selection

Compared methods for explainability & performance:
- Mutual Information
- Chi-Square Test
- ANOVA (F-value)
- Random Forest Feature Importance
- Recursive Feature Elimination (RFE)

---

## Modeling & Evaluation

**Algorithms:**
- Decision Tree
- Random Forest
- Support Vector Machine (SVM)
- Logistic Regression
- Naive Bayes

**Steps:**
- GridSearchCV (3-fold) for tuning
- Test set evaluation

**Metrics:**  
Accuracy, F1, Precision, Recall, Confusion Matrix

---

## Results & Insights

- **Best test accuracy:** 95.6%
- **Most important features:** ['FunctionalAssessment', 'ADL', 'MMSE', 'MemoryComplaints_encoded', 'PatientID',]
- **SMOTE** improved minority class performance
- See details & charts in [`presentation.pdf`](presentation.pdf)

---

## Presentation

Summary of workflow, methods, and results in [`presentation.pdf`](presentation.pdf) (Persian, with tables & diagrams).

---

## How to Run

1. **Clone this repo:**
    ```bash
    git clone https://github.com/Arianafshar2003/Alzheimers-Diseases-Classification.git
    cd Alzheimers-Diseases-Classification
    ```
2. **Open notebook:**  
   - Use Jupyter Notebook or Google Colab  
3. **Install dependencies:**  
    ```bash
    pip install -r requirements.txt
    ```
    *(If you need requirements.txt, see below!)*
4. **(Optional) Download data:**  
   - See notebook instructions for Kaggle download  
5. **Run all cells & review outputs**

---

## Acknowledgements

- **Instructor:** Dr. Baghdadi  
- **Course:** Machine Learning, Amirkabir University of Technology (Tehran Polytechnic)

---

## توضیحات فارسی برای دانشجویان و اساتید ایرانی

این پروژه شامل کل فرایند داده‌کاوی: تحلیل اکتشافی، پیش‌پردازش، انتخاب ویژگی، مدل‌سازی و ارزیابی بر اساس دیتاست بیماران آلزایمری است. اسلایدها و توضیحات تکمیلی در [presentation.pdf](presentation.pdf) آمده است. برای اجرا کافیست فایل نوت‌بوک را در ژوپیتر یا گوگل‌کولب باز و مراحل را دنبال کنید.

---

