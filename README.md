# Fraudulent Job Detection Using Machine Learning

## Overview

Employment scams have become increasingly common with the rise of online recruitment platforms. Fraudsters often post fake job advertisements that closely resemble legitimate opportunities, with the intention of extracting money or sensitive personal information such as bank details, identity proofs, or contact information from job seekers.

This project presents a **machine learning–based approach** to identify fraudulent job postings by analyzing both **textual content** and **structured attributes** of job advertisements. The system classifies job postings as **real or fraudulent** using supervised learning techniques and natural language processing (NLP).

---

## Problem Definition

The objective of this project is to build a reliable classification model capable of detecting fraudulent job postings from real-world recruitment data. Since fraudulent listings are relatively rare compared to genuine job postings, the problem involves handling **class imbalance** while maintaining good predictive performance.

---

## Model Description

**Fraudulent-Job-Detection-Using-ML** is implemented in Python and uses machine learning algorithms to analyze job postings.

The following models are used:
- **Multinomial Naive Bayes**
- **Decision Tree Classifier**

Textual data from job postings is preprocessed using NLP techniques and converted into numerical representations for model training. Model performance is evaluated using accuracy and confusion matrices.

Detailed analysis, preprocessing steps, and model implementation can be found in the Jupyter notebook:

📄 `Fake_job_predictor.ipynb`

<p align="center">
  <img width="460" height="300" src="Images/image1.PNG">
</p>

---

## Technology Stack

- Python  
- NumPy  
- Pandas  
- Matplotlib  
- Scikit-learn  
- Natural Language Toolkit (NLTK)  
- WordCloud  
- Imbalanced-learn  
- Flask  

---

## Dataset

The project uses the **Employment Scam Aegean Dataset (EMSCAD)**, which contains labeled job postings marked as real or fraudulent.

Dataset source:  
https://www.kaggle.com/amruthjithrajvr/recruitment-scam

The dataset includes job-related attributes such as:
- Job title and description  
- Company profile  
- Location and experience requirements  
- Fraud label  

---

## Exploratory Data Analysis

### Job Distribution by Location
<p align="center">
  <img width="460" height="300" src="Images/image2.PNG">
</p>

### Job Distribution by Experience Level
<p align="center">
  <img width="460" height="300" src="Images/image3.PNG">
</p>

### WordCloud of Common Terms
<p align="center">
  <img width="460" height="300" src="Images/image4.PNG">
</p>

Exploratory analysis helps identify trends and patterns that differentiate fraudulent postings from genuine ones.

---

## Model Evaluation

### Multinomial Naive Bayes
- **Accuracy:** 0.898  

<p align="center">
  <img width="460" height="300" src="Images/image5.PNG">
</p>

---

### Decision Tree Classifier
- **Accuracy:** 0.817  

<p align="center">
  <img width="460" height="300" src="Images/image6.PNG">
</p>

---

## Results

- Naive Bayes achieved better overall performance compared to the Decision Tree classifier.
- Text-based features played a significant role in identifying fraudulent postings.
- Class imbalance remains a key challenge in fraud detection tasks.

---

## Limitations

- The dataset is highly imbalanced, with fewer fraudulent samples.
- Some fraudulent postings closely resemble legitimate job advertisements.
- Decision Tree models showed lower generalization performance.

---

## Future Scope

- Apply oversampling techniques such as SMOTE
- Explore ensemble and deep learning models
- Improve recall for fraudulent job detection
- Deploy the model using modern cloud platforms

---

## Disclaimer

This project is developed for academic and learning purposes using publicly available data. The results are intended for research and educational use only.
