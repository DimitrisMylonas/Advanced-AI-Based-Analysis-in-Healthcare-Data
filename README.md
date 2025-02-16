# Advanced AI-Based Analysis in Healthcare Data

## Overview
This project focuses on applying advanced AI-based methodologies for analyzing healthcare data, specifically targeting **cardiovascular disease (CVD) prediction**. The study utilizes **machine learning techniques** to improve classification performance by handling class imbalance, incorporating cost-sensitive learning, and enhancing interpretability.

## Dataset
- **Cardiovascular Disease Dataset** sourced from Kaggle
- **70,000 patient records**
- **11 Features + 1 Target Variable**
- Feature categories:
  - **Objective**: Age, height, weight, gender
  - **Medical Examination**: Systolic & Diastolic Blood Pressure, Cholesterol, Glucose
  - **Subjective**: Smoking, Alcohol Intake, Physical Activity
- **Goal**: Predict the presence or absence of CVD using machine learning models

## Methodology
The methodology applied in this project includes:
1. **Data Preprocessing & Cleaning**
   - Removal of outliers based on quantiles (0.025 - 0.975)
   - Feature transformation and encoding for machine learning compatibility

2. **Class Imbalance Handling**
   - **SMOTE** (Synthetic Minority Oversampling Technique)
   - **Near Miss** (Undersampling Majority Class)
   - **Cost-Sensitive Learning** (Weighting Loss Function)

3. **Cost-Sensitive Learning Techniques**
   - **Weighting**: Assigning different costs for misclassifications
   - **Resampling**: Combining Oversampling & Undersampling
   - **Isotonic Calibration**: Adjusting probability estimates for better performance

4. **Active Learning**
   - Uncertainty Sampling: Least Confidence Sampling to improve model training with limited labeled data

5. **Interpretability**
   - **Global Interpretation**
     - Feature Importance Analysis
     - SHAP (SHapley Additive exPlanations)
     - Weight Plotting
   - **Local Interpretation**
     - LIME (Local Interpretable Model-Agnostic Explanations)

## Results
- **Cost-Sensitive Learning** reduced misclassification costs across all tested classifiers
- **Class Imbalance Techniques** significantly improved false-positive predictions
- **Active Learning** showed minor improvements but was not optimal for cost reduction
- **Interpretability Analysis** highlighted key risk factors such as systolic blood pressure and age as the primary predictors of cardiovascular disease.

## Future Work
- Extend the study to other healthcare datasets to validate findings
- Improve **Active Learning** techniques for more efficient data labeling
- Implement deep learning-based approaches for comparison with traditional ML models
- Investigate **causal inference** to understand patient risk factors more deeply

## Authors
- **Dimitrios Mylonas** - MSc in Data & Web Science, Aristotle University of Thessaloniki
- **Dimitrios Sainidis** - MSc in Data & Web Science, Aristotle University of Thessaloniki
- **Dimitrios Valsamis** - MSc in Artificial Intelligence, Aristotle University of Thessaloniki
