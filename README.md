# Pneumonia Detection using Deep Learning

A deep learning project for automated **Pneumonia Detection from Chest X-ray Images** using multiple CNN and transfer learning architectures including **Custom CNN, MobileNetV2, ResNet18, and DenseNet121**.

The project compares model performance using various evaluation metrics to identify the most effective architecture for medical image classification.

---

## Project Overview

Pneumonia is a serious respiratory disease that can be life-threatening if not diagnosed early. Manual diagnosis through chest X-rays requires experienced radiologists and can be time-consuming.

This project uses **Deep Learning** techniques to automatically classify chest X-ray images into:

- **Normal**
- **Pneumonia**

The study applies:
- Image preprocessing
- Data augmentation
- Transfer learning
- Class imbalance handling
- Multi-model comparison

using the **Chest X-ray Pneumonia Dataset**.

---

## 🛠 Technologies Used

- Python
- TensorFlow / Keras
- PyTorch
- OpenCV
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

---

## Dataset

Dataset used:
- **Chest X-ray Pneumonia Dataset (Kermany Dataset)**
- Approximately **5,856 chest X-ray images**

Classes:
- NORMAL
- PNEUMONIA

Dataset includes:
- Training set
- Validation set
- Test set

---

## 🧠 Models Implemented

### 1. Custom CNN
A CNN built from scratch using:
- Conv2D
- MaxPooling
- Dropout
- Dense layers

Features:
- CLAHE preprocessing
- Binary classification using sigmoid activation

---

### 2. MobileNetV2
Transfer learning model using pretrained ImageNet weights.

Features:
- Depthwise separable convolutions
- Lightweight architecture
- Two-phase fine tuning

---

### 3. ResNet18
PyTorch implementation using residual connections.

Features:
- AdamW optimizer
- CosineAnnealingLR scheduler
- BCEWithLogitsLoss

---

### 4. DenseNet121 (Best Model)
Best performing model in the project.

Features:
- Dense connectivity
- Efficient feature reuse
- Mixed precision training
- Two-phase fine tuning

---

## 🔄 Workflow

1. Data Loading
2. Image Preprocessing
3. Data Augmentation
4. Model Training
5. Fine Tuning
6. Evaluation
7. Comparative Analysis

---

## Image Preprocessing

The following preprocessing techniques were used:
- Image resizing (224×224)
- Normalization
- CLAHE enhancement
- Rotation
- Zoom
- Horizontal flipping
- Brightness adjustment

---

##  Evaluation Metrics

Models were evaluated using:
- Accuracy
- Precision
- Recall (Sensitivity)
- Specificity
- F1-score
- AUC Score
- Confusion Matrix

---

## 📈 Final Results

| Model | Accuracy | AUC | Sensitivity | Specificity | F1 Score |
|---|---|---|---|---|---|
| Custom CNN | 73.08% | 0.791 | 77.95% | 64.96% | 0.73 |
| MobileNetV2 | 89.74% | 0.974 | 97.95% | 76.07% | 0.89 |
| ResNet18 | 83.81% | 0.87 | 99.23% | 58.12% | 0.83 |
| DenseNet121 ⭐ | 90.87% | 0.959 | 96.15% | 82.05% | 0.91 |

---

##  Best Model

### DenseNet121
DenseNet121 achieved:
- Highest Accuracy
- Highest F1-score
- Lowest Test Loss
- Best balance between sensitivity and specificity

It was selected as the recommended model for pneumonia screening deployment.

---

## 📌 Key Insights

- Transfer learning significantly outperformed the custom CNN.
- Proper validation split improved generalization.
- ResNet18 achieved extremely high recall but produced more false positives.
- DenseNet121 provided the best overall balance.

---

## 🚀 Future Improvements

Possible future enhancements:
- Vision Transformers (ViT)
- Larger medical datasets
- Explainable AI (Grad-CAM)
- Real-time deployment
- Multi-class lung disease classification

---

## 📚 References

1. CheXNet — Rajpurkar et al.
2. Kermany et al. — Deep Learning for Medical Diagnosis
3. ChestX-ray14 Dataset — Wang et al.
4. Transfer Learning for Pneumonia Detection — Chouhan et al.

---

## 📄 Project Description

This project demonstrates how deep learning and transfer learning techniques can assist in early pneumonia detection using chest X-ray images, helping improve diagnostic efficiency and healthcare accessibility.
