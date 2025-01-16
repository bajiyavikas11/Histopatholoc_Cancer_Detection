## Overview

This project focuses on detecting metastatic cancer in histopathologic images using various machine learning techniques. By leveraging data preprocessing, augmentation, and multiple models, we aimed to classify image patches as cancerous or non-cancerous with high accuracy. The project highlights the use of advanced AI techniques to improve early cancer detection, aiding in timely diagnosis and treatment planning.

## Objectives

1. Binary Classification: Classify 32x32-pixel histopathologic image patches as positive (cancerous) or negative (non-cancerous).
2. Model Development: Design, train, and evaluate six machine learning models for performance comparison.
3. Efficiency and Accuracy: Optimize models to achieve the highest accuracy while addressing data imbalance.

## Dataset

1. Source: https://www.kaggle.com/competitions/histopathologic-cancer-detection

2. Classes:
            Label 0: Negative (no cancer).
            Label 1: Positive (cancer present).
   
3. Key Characteristics:
            Contains ~220,000 labeled images.
            Imbalanced distribution (more negatives than positives).

4. Preprocessing:
            Normalization and standardization.
            Synthetic Minority Oversampling Technique (SMOTE) for class imbalance.
            Data augmentation (random flips, rotations, resizing).

## Models Implemented

1. Naive Bayes
            Accuracy: 73%
            Strengths: Efficiency for large datasets.
2. Random Forest
            Accuracy: 75%
            Captures non-linear relationships effectively.
3. Logistic Regression
            Accuracy: 63%
            Includes probability calibration with isotonic regression.
4. Support Vector Machine (SVM)
            Accuracy: 76%
            Uses kernel functions for non-linear decision boundaries.
5. Neural Network (Improved Architecture)
            Accuracy: 77%
            Features dropout layers, AdamW optimizer, and SMOTE handling.
6. XGBoost
            Accuracy: 81%
            Best performer in terms of accuracy, precision, recall, and F1-score.
   
## Results

Model	                  Accuracy	    Precision	    Recall	    F1-score
Naive Bayes	            73%	          75%	          73%	        73%
Random Forest	          75%	          76%	          75%	        74%
Logistic Regression	    63%	          62%	          63%	        62%
Support Vector Machine	76%	          77%	          76%	        77%
Neural Network	        77%	          77%	          77%	        77%
XGBoost	                81%	          81%	          81%	        81%
