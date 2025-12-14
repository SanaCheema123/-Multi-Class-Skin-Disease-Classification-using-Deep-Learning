# 🩺 Multi-Class Skin Disease Classification using Deep Learning

This repository presents a **deep learning–based multi-class skin disease classification system** developed using **transfer learning with EfficientNetB0**. The model is trained on a publicly available dermatology image dataset and achieves **high classification accuracy** through fine-tuning, data augmentation, and robust training strategies.

---

## 📌 Project Overview

Skin diseases vary significantly in appearance, making automated diagnosis a challenging task. This project aims to assist in **early and accurate identification of multiple skin conditions** using convolutional neural networks (CNNs).

The system leverages **EfficientNetB0**, a state-of-the-art lightweight CNN architecture, fine-tuned on a multi-class skin condition dataset to deliver reliable performance.

---

## 📊 Dataset

- **Dataset Name:** Multi-Class Skin Condition Image Dataset (MSC-6)
- **Source:** Kaggle  
- **Link:** https://www.kaggle.com/datasets/harishnivasagam/multi-class-skin-condition-image-dataset-msc-6
- **Description:**  
  The dataset contains labeled images of **six different skin conditions**, suitable for supervised multi-class classification tasks.

---

## 🧠 Model Architecture

- **Base Model:** EfficientNetB0 (pretrained on ImageNet)
- **Approach:** Transfer Learning + Fine-Tuning
- **Classifier Head:** Custom fully connected layers added on top of the base model
- **Loss Function:** Categorical Cross-Entropy
- **Optimizer:** Adam

EfficientNetB0 was selected due to its **high accuracy-to-parameter ratio**, making it well-suited for medical image classification.

---

## 🔧 Training Techniques

To enhance performance and generalization, the following techniques were applied:

### ✅ Data Augmentation
- Random rotations
- Horizontal and vertical flips
- Zoom transformations
- Image rescaling

### ✅ Regularization & Optimization
- **EarlyStopping** callback to prevent overfitting
- Fine-tuning of top layers of EfficientNet
- Reduced learning rate during fine-tuning

---

## 📈 Training Results

The model was trained for **25 epochs**, achieving excellent performance:

