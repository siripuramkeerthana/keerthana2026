# keerthana2026
# Predicting Brain Stroke Risk Using Hybrid Machine Learning and Deep Learning Models

## Overview
Brain stroke is one of the leading causes of death and long-term disability worldwide. Early detection is critical to reduce mortality and improve patient outcomes.

This project focuses on developing an automated brain stroke prediction system using **Hybrid Machine Learning and Deep Learning models** to classify brain scan images into:

- **Stroke**
- **No Stroke**

The project compares the performance of:

- Custom Convolutional Neural Network (CNN)
- ResNet101 (Transfer Learning)
- DenseNet201 (Transfer Learning)

The system also uses **Grad-CAM visualization** to improve model interpretability by highlighting important regions in brain images during prediction.

---

## Project Objectives

- Develop an intelligent system for brain stroke prediction
- Compare machine learning and deep learning models
- Improve prediction accuracy using transfer learning techniques
- Handle class imbalance issues
- Apply image preprocessing and augmentation techniques
- Use explainable AI techniques for model transparency

---

## Dataset

The dataset was collected from:

**Hugging Face – BTX24 Brain Stroke Dataset**

### Dataset Details

| Feature | Description |
|----------|-------------|
| Classes | Stroke / No Stroke |
| Data Type | Brain Medical Images |
| Image Format | JPG |
| Image Size | 224x224 |
| Split Ratio | Train (80%), Validation (10%), Test (10%) |

### Challenges
- Class imbalance
- Limited dataset size
- Mixed grayscale and RGB images
- Image quality variations

---

## Technologies Used

### Programming Language
- Python

### Libraries & Frameworks
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- OpenCV
- Hugging Face Datasets

---

# Project Workflow

## 1. Data Collection
- Download dataset from Hugging Face
- Organize into train/validation/test sets

## 2. Data Preprocessing
- Resize images to 224x224
- Normalize pixel values
- Convert RGBA images to RGB
- Handle class imbalance using class weights

## 3. Data Augmentation
Applied:
- Rotation
- Zoom
- Horizontal flipping
- Width shifting
- Height shifting

## 4. Feature Extraction
Using:
- CNN
- ResNet101
- DenseNet201

## 5. Model Training
Models trained using:
- Adam Optimizer
- Categorical Crossentropy Loss
- Early Stoppin

## 6. Model Evaluation
Metrics used:
- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

## 7. Explainability
- Grad-CAM visualization

---

# Model Architectures

## Custom CNN
- Conv2D
- Batch Normalization
- MaxPooling
- Dropout
- Dense Layers
- Softmax Output

---

## ResNet101
Pretrained on ImageNet:
- Frozen base layers
- Global Average Pooling
- Dense Layer
- Dropout
- Softmax Output

---

## DenseNet201
Pretrained on ImageNet:
- Frozen base layers
- Global Average Pooling
- Dense Layer
- Dropout
- Softmax Output

---

# Results

| Model       | Accuracy | Precision | Recall | F1 Score |
|-------------|----------|-----------|--------|----------|
| CNN         | ~60.37%  | 0.60      | 0.60   | 0.59     |
| ResNet101   | ~72.99%  | 0.72      | 0.72   | 0.69     |
| DenseNet201 | ~93%     | 0.92      | 0.91   | 0.91     |

---

## Best Performing Model
✅ **DenseNet201**

DenseNet201 achieved the highest performance due to:

- Better feature reuse
- Strong gradient flow
- Higher classification accuracy
- Better generalization capability

---

# Grad-CAM Visualization

Grad-CAM was used to visualize:

- Which areas of the brain image influenced predictions
- Stroke affected regions
- Model decision-making transparency

This helps improve trust in AI-based medical diagnosis systems.


Author

Keerthana Siripuram
Master in Computer Science
University of East London

Supervisor: Farrah Aftab
