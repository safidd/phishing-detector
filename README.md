# Phishing Website Detector

A machine learning classifier that detects phishing websites using Random Forest algorithm, achieving **97% accuracy** on a dataset of 11,000+ websites.

## Overview

Phishing attacks trick users into visiting fake websites that steal credentials or install malware. This project builds a binary classifier that identifies whether a website is phishing or legitimate based on 30 URL and page features.

## Dataset

- **Source:** Kaggle - Phishing Website Detector
- **Size:** 11,054 websites
- **Features:** 30 binary/ternary encoded features (1, 0, -1)
- **Target:** class — 1 (legitimate) or -1 (phishing)
- **Class distribution:** 6,157 legitimate / 4,897 phishing

## Model

- **Algorithm:** Random Forest (100 estimators)
- **Train/Test Split:** 80% / 20%

## Results

| Metric | Phishing (-1) | Legitimate (1) |
|---|---|---|
| Precision | 0.97 | 0.97 |
| Recall | 0.96 | 0.98 |
| F1-Score | 0.96 | 0.97 |
| Accuracy | 0.97 | |

## Key Findings

- HTTPS and AnchorURL are the two most important features
- Only 39 phishing sites missed out of 976
- False negative rate of 4%

## Real-World Applications

- Browser extensions for real-time URL scanning
- Email security filters
- Corporate firewall URL filtering
- SOC triage tools

## How to Run

pip install pandas scikit-learn matplotlib seaborn
python3 phishing_detector.py

## Skills Demonstrated

Python, Scikit-learn, Random Forest, Data Preprocessing, Model Evaluation, Cybersecurity, Machine Learning
