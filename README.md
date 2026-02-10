# ECG Arrhythmia Detection using Signal Processing and Machine Learning

> Part of the Healthcare Data Science Portfolio  
> https://github.com/Bananas723/healthcare-data-science-portfolio

## Overview

This project demonstrates an end-to-end data science workflow for the analysis of electrocardiogram (ECG) signals with the goal of detecting cardiac arrhythmias. The focus is on combining classical biomedical signal processing with machine learning methods, reflecting typical real-world applications in healthcare technology.

The project is designed as a compact but realistic portfolio example for data science and AI roles in the medical and health technology domain.

---

## Objectives

* Preprocess raw ECG signals and reduce noise and artifacts
* Extract clinically relevant features from ECG time series
* Train and evaluate machine learning models for arrhythmia classification
* Assess model performance using appropriate metrics for imbalanced medical data

---

## Dataset

* Publicly available ECG dataset (e.g. MIT-BIH Arrhythmia Database)
* Signals sampled at fixed frequency
* Beat-level or segment-level annotations provided

> Note: Only publicly available and anonymized data is used.

---

## Methods

### Signal Processing

* Bandpass filtering to remove baseline wander and high-frequency noise
* R-peak detection (e.g. Pan–Tompkins algorithm)
* Segmentation of ECG signals into individual heartbeats

### Feature Engineering

* Time-domain features (RR intervals, heart rate variability)
* Morphological features (QRS duration, amplitudes)
* Statistical features (mean, variance, skewness)

### Machine Learning

* Baseline models: Logistic Regression, k-Nearest Neighbors
* Advanced models: Random Forest, Support Vector Machine
* Optional extension: 1D Convolutional Neural Network

---

## Evaluation

* Train/test split with patient-wise separation
* Metrics:

  * Accuracy
  * Precision, Recall, F1-score
  * Confusion Matrix
* Discussion of class imbalance and clinical relevance of false positives vs. false negatives

---

## Results

* Comparison of classical ML models
* Analysis of feature importance
* Interpretation of results from a clinical perspective

> The goal is not maximum performance, but methodological correctness and interpretability.

---

## Technologies Used

* Python
* NumPy, Pandas
* SciPy (signal processing)
* scikit-learn
* Matplotlib / Seaborn

---

## Project Structure

```
ecq-arrhythmia-detection/
├── data/            # Raw and processed ECG data
├── notebooks/       # Exploratory analysis and experiments
├── src/             # Reusable preprocessing and modeling code
├── results/         # Figures and evaluation outputs
├── README.md
```

---

## Background

This project is part of a personal portfolio in healthcare data science.

Academic background:

* B.Sc. Medical Engineering
* Bachelor thesis: "Prediction of Sepsis in ICU Patients using Deep Learning – A Case Study based on the MIMIC Database"

---

## Future Extensions

* Deep learning-based ECG classification (CNN, LSTM)
* Multi-lead ECG analysis
* Explainability methods (e.g. SHAP, saliency maps)

---

## Disclaimer

This project is for educational and research purposes only and does not constitute medical advice or a certified medical device.
