# Fraudulent Job Detection Using Machine Learning

## Problem Statement

Employment scams closely imitate legitimate job advertisements by appearing on job portals, social media platforms, newspapers, and other online channels. These scams typically promise attractive job opportunities but are designed to steal money or sensitive personal information such as bank details, identity documents, or contact information.

With the rapid growth of online recruitment platforms, detecting fraudulent job postings has become a critical challenge. This project addresses the problem by applying machine learning and natural language processing techniques to automatically classify job postings as **real or fraudulent**.

---

## Model Description

**Fraudulent-Job-Detection-Using-ML** is a Python-based machine learning system that predicts whether a job posting is genuine or fake. The model leverages both textual and structured features extracted from job advertisements.

The following algorithms are used:
- **Multinomial Naive Bayes**
- **Decision Tree Classifier**

The complete exploratory analysis, feature engineering, and model development are documented in the Jupyter notebook:

📄 `Fake_job_predictor.ipynb`

> Note: Deployment references (e.g., Heroku) are excluded to keep this repository focused on model development and analysis.

<p align="center">
  <img width="460" height="300" src="Images/image1.PNG">
</p>

---

## Technology Stack & Libraries

- Python
- NumPy
- Pandas
- Matplotlib
- Imbalanced-learn
- Natural Language Toolkit (NLTK)
- WordCloud
- Scikit-learn
  - Multinomial Naive Bayes
  - Decision Tree Classifier
- Flask (for API-level experimentation)

---

## Dataset Description

This project uses the **Employment Scam Aegean Dataset (EMSCAD)**, which contains labeled job postings categorized as real or fraudulent.

Dataset source:  
https://www.kaggle.com/amruthjithrajvr/recruitment-scam

The dataset includes:
- Job titles
- Company information
- Job descriptions
- Experience requirements
- Location details
- Fraud labels

---

## Exploratory Data Analysis

### Job Distribution by Location

<p align="center">
  <img width="460" height="300" src="Images/image2.PNG">
</p>

---

### Job Distribution by Experience Level

<p align="center">
  <img width="460" height="300" src="Images/image3.PNG">
</p>

---

### WordCloud Visualization of Common Terms

<p align="center">
  <img width="460" height="300" src="Images/image4.PNG">
</p>

WordCloud analysis highlights frequently used terms in fraudulent job postings, helping identify suspicious language patterns.

---

## Model Evaluation

### Multinomial Naive Bayes

Multinomial Naive Bayes is used as a baseline classifier due to its effectiveness in handling categorical text data.

- **Accuracy:** 0.898  
- **Confusion Matrix:**

<p align="center">
  <img width="460" height="300" src="Images/image5.PNG">
</p>

---

### Decision Tree Classifier

The Decision Tree classifier segments the feature space into decision regions based on information gain.

- **Accuracy:** 0.817  
- **Confusion Matrix:**

<p align="center">
  <img width="460" height="300" src="Images/image6.PNG">
</p>

---

## Results & Observations

- Naive Bayes outperformed the Decision Tree classifier in terms of accuracy.
- Textual features played a major role in identifying fraudulent postings.
- Class imbalance significantly affects fraud recall, requiring careful metric selection.

---

## Limitations

- Dataset is highly imbalanced (few fraudulent samples).
- Decision Trees showed lower generalization performance.
- Some fraudulent postings closely resemble legitimate listings.

---

## Future Enhancements

- Apply oversampling techniques such as **SMOTE**
- Experiment with ensemble models
- Use TF-IDF with advanced NLP embeddings
- Improve recall for minority (fraudulent) class
- Deploy using modern platforms (Docker / cloud-native services)

---

## Disclaimer

This repository represents an independently maintained academic and research-oriented implementation developed for learning and experimentation purposes.
