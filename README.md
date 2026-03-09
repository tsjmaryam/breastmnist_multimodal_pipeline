# BreastMNIST Multimodal Pipeline for Breast Cancer Classification

## Overview
This repository implements a deep learning pipeline for breast cancer classification using the BreastMNIST dataset. The project explores convolutional neural networks (CNNs) for medical image analysis and integrates model evaluation metrics commonly used in clinical research, including accuracy, ROC-AUC, and confusion matrix analysis.

The objective is to investigate how deep learning models can assist in early detection of malignant breast tumors while maintaining transparency in performance reporting.

This project is part of my ongoing work in AI for healthcare and responsible machine learning.

---

## Dataset
The project uses the BreastMNIST dataset, part of the MedMNIST benchmark collection for lightweight biomedical image classification.

Dataset characteristics:

- **Task:** Binary classification (benign vs malignant)
- **Image size:** 28 × 28 grayscale images
- **Source:** Breast ultrasound images
- **Dataset split:** Training, Validation, Test

Reference:  
MedMNIST: A Lightweight Benchmark for 2D and 3D Biomedical Image Classification

---

## Model Architecture
The model is a Convolutional Neural Network (CNN) designed to learn spatial features from breast ultrasound images.

Key components:

- Convolutional layers for feature extraction
- Max pooling layers for spatial down-sampling
- Fully connected layers for classification
- Sigmoid output layer for binary prediction

The pipeline includes:

- Data loading and preprocessing
- Model training
- Evaluation using multiple performance metrics
- Visualization of prediction results

---

## Evaluation Metrics
Model performance is evaluated using:

- Test Accuracy
- ROC-AUC Score
- Confusion Matrix

Particular attention is given to **false negatives**, where malignant tumors are incorrectly classified as benign. In clinical screening scenarios, minimizing false negatives is critical because missed cancer cases can delay treatment.

---

## Tech Stack

### Programming
Python

### Deep Learning
PyTorch  
Torchvision

### Medical Imaging Dataset
MedMNIST (BreastMNIST)

### Machine Learning & Evaluation
Scikit-learn  
NumPy

### Large Language Models
Qwen (via HuggingFace Transformers)

### Visualization
Matplotlib

### Utilities
tqdm (training progress monitoring)  
Requests

### Development Environment
Google Colab

---

## Repository Structure

```
breastmnist_multimodal_pipeline/
│
├── breastmnist_pipeline.ipynb     # Main training and evaluation notebook
└── README.md                      # Project documentation
```


## Key Results

Example baseline model results:

- **Test Accuracy:** ~73%
- **ROC-AUC:** ~0.78

The confusion matrix analysis highlights the balance between correctly detecting malignant cases and avoiding false negatives.

These results demonstrate the feasibility of lightweight CNN architectures for breast cancer image classification while emphasizing the importance of careful evaluation in medical AI applications.

---

## Future Improvements
Potential extensions of this work include:

- Incorporating transfer learning architectures
- Adding explainability methods (Grad-CAM / SHAP for CNNs)
- Testing larger medical imaging datasets
- Integrating multimodal clinical features

---

## Author
Maryam Shahbaz Ali  
