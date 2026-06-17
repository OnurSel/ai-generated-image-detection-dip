# AI-Generated Image Detection Using Digital Image Processing and Machine Learning

This project implements a lightweight and interpretable framework for detecting AI-generated images using handcrafted digital image processing features and machine learning.

## Overview

The goal of this project is to classify images as:

- **REAL**: real photographs
- **FAKE**: AI-generated synthetic images

The system extracts handcrafted image features and evaluates both an external baseline classifier and the proposed SVM-based classifier.

## Methods Used

Feature extraction techniques:

- Local Binary Pattern (LBP)
- Fast Fourier Transform (FFT)
- Gray-Level Co-occurrence Matrix (GLCM)
- Sobel Edge Analysis

Machine learning models:

- Logistic Regression baseline
- Support Vector Machine (SVM) proposed model

## Dataset

The project uses the CIFAKE dataset:

https://www.kaggle.com/datasets/birdy654/cifake-real-and-ai-generated-synthetic-images

## Experimental Setup

- Platform: Google Colab
- Language: Python
- Libraries: OpenCV, NumPy, Scikit-image, Scikit-learn, Matplotlib
- Train-test split: 80/20
- Hyperparameter tuning: GridSearchCV with 5-fold cross-validation

## Best SVM Parameters

- Kernel: RBF
- C: 10
- Gamma: 0.01

## Repository Contents

```text
AI_Generated_Image_Detection_COMP430_FINAL_REVISED.ipynb
README.md
```

## How to Run

1. Open the notebook in Google Colab.
2. Run all cells from top to bottom.
3. The dataset will be downloaded automatically using `kagglehub`.
4. The notebook performs feature extraction, baseline comparison, SVM optimization, and final evaluation.

## Author

Onur Sel  
Department of Computer Engineering  
Abdullah Gül University
