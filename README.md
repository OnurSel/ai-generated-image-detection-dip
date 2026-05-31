# AI-Generated Image Detection Using Digital Image Processing and Machine Learning

This project implements a lightweight and interpretable framework for detecting AI-generated images using handcrafted digital image processing features and machine learning.

## Project Overview

The goal of this project is to classify images as either:

- **REAL**: real photographs
- **FAKE**: AI-generated synthetic images

The system extracts handcrafted image features and uses a Support Vector Machine (SVM) classifier for final prediction.

## Methods Used

The following digital image processing techniques were used for feature extraction:

- **Local Binary Pattern (LBP)** for texture analysis
- **Fast Fourier Transform (FFT)** for frequency-domain analysis
- **Gray-Level Co-occurrence Matrix (GLCM)** for statistical texture features
- **Sobel Edge Analysis** for gradient and edge-based features

## Dataset

The project uses the **CIFAKE: Real and AI-Generated Synthetic Images Dataset** from Kaggle.

Dataset link:  
https://www.kaggle.com/datasets/birdy654/cifake-real-and-ai-generated-synthetic-images

## Experimental Setup

- Platform: Google Colab
- Programming language: Python
- Libraries:
  - OpenCV
  - NumPy
  - Scikit-image
  - Scikit-learn
  - Matplotlib

The dataset was split into training and testing sets using an 80/20 split.

## Model

A Support Vector Machine (SVM) classifier was used.

Hyperparameter tuning was performed using GridSearchCV with 5-fold cross-validation.

Best parameters:

- Kernel: RBF
- C: 10
- Gamma: 0.01

## Results

The final model achieved:

| Metric | Value |
|---|---|
| Accuracy | 84.5% |
| Precision | 0.825 |
| Recall | 0.850 |
| F1-score | 0.837 |
| AUC Score | 0.902 |

## Feature Comparison

| Feature Set | Accuracy | F1-score |
|---|---|---|
| LBP Only | 66.5% | 0.663 |
| FFT Only | 70.0% | 0.703 |
| GLCM Only | 73.0% | 0.735 |
| Edge Only | 73.5% | 0.741 |
| Combined Features | 84.5% | 0.839 |

## Repository Contents

```text
AI_Generated_Image_Detection_COMP430_FINAL.ipynb
README.md
