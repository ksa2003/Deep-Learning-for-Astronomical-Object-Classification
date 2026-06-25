# Deep Learning for Astronomical Object Classification

## Overview

This project focuses on the automatic classification of astronomical objects using data from the Sloan Digital Sky Survey (SDSS).

The objective is to build and compare Machine Learning and Deep Learning models capable of identifying celestial objects as:

* Stars
* Galaxies
* Quasars

The project follows an end-to-end Data Science workflow, from data acquisition and exploratory analysis to model deployment and evaluation.

---

## Problem Statement

Modern astronomical surveys generate massive amounts of observational data. Manual classification of celestial objects is no longer feasible at scale.

The goal of this project is to develop automated classification systems capable of accurately distinguishing stars, galaxies, and quasars using photometric and spectroscopic measurements.

---

## Dataset

### Sloan Digital Sky Survey (SDSS)

Source:

* SDSS Data Release 17
* Kaggle SDSS Stellar Classification Dataset

Features include:

* Right Ascension (RA)
* Declination (DEC)
* Redshift (z)
* Spectroscopic measurements
* Photometric magnitudes (u, g, r, i, z)

Target classes:

* STAR
* GALAXY
* QSO (Quasar)

---

## Project Structure

```text
.
├── data/
│   ├── raw/
│   ├── processed/
│
├── notebooks/
│   ├── 01_eda.ipynb
│   ├── 02_preprocessing.ipynb
│   ├── 03_machine_learning.ipynb
│   ├── 04_deep_learning.ipynb
│
├── models/
│
├── src/
│   ├── data.py
│   ├── preprocessing.py
│   ├── model.py
│   ├── registry.py
│
├── tests/
│
├── requirements.txt
│
└── README.md
```

---

## Exploratory Data Analysis

The analysis includes:

* Class distribution
* Feature distributions
* Correlation analysis
* Missing values inspection
* Outlier detection
* Dimensionality reduction (PCA, t-SNE)

---

## Data Preprocessing

Main preprocessing steps:

* Missing value handling
* Feature scaling
* Feature engineering
* Class balancing
* Train / Validation / Test split
* Stratified sampling

---

## Machine Learning Models

The following baseline models are evaluated:

### Logistic Regression

* Fast baseline
* Interpretable coefficients

### Random Forest

* Ensemble learning
* Feature importance analysis

### XGBoost

* Gradient boosting
* High predictive performance

### Support Vector Machine (SVM)

* Effective in high-dimensional spaces

---

## Deep Learning Models

### Fully Connected Neural Network (MLP)

Architecture:

```text
Input Layer
    ↓
Dense Layers
    ↓
Output Layer
```

### Deep Neural Networks

* Batch Normalization
* Dropout Regularization
* Early Stopping

---

## Evaluation Metrics

The models are evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* Macro F1-score
* Confusion Matrix

Special attention is given to Macro F1-score to ensure balanced performance across all classes.

---

## Results

The final comparison includes:

| Model               | Accuracy | Macro F1 |
| ------------------- | -------- | -------- |
| Logistic Regression |          |          |
| Random Forest       |          |          |
| XGBoost             |          |          |
| SVM                 |          |          |
| Neural Network      |          |          |

---

## Technologies

* Python
* Pandas
* NumPy
* Scikit-Learn
* TensorFlow / Keras
* XGBoost
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## Future Work

Potential extensions:

* Vision Transformers (ViT)
* Convolutional Neural Networks on SDSS images
* Multi-modal learning combining tabular and image data
* Explainable AI (SHAP, LIME)
* Real-time astronomical object classification

---

## Authors

Data Science Project

2026

