# 🧠 CNN Multi-Class Classifier – Digits, Letters & Math Symbols

This project implements a **Convolutional Neural Network (CNN)** to classify images of:
- Digits (0–9)
- English letters (W, X, Y, Z)
- Mathematical operators: `+`, `-`, `/`, and `*` (represented as a dot `.`)

The model is trained and evaluated using a **custom dataset**, where each image's class is derived from its filename. This project covers an end-to-end machine learning pipeline using **PyTorch**.

---

## 📂 Dataset Overview

- **Source**: Provided as a ZIP file containing images
- **Classes**: 14 total
- **Format**: Each image's label is encoded in the filename
- **Goal**: Multi-class classification using a CNN model

---

## ✅ Project Tasks

### 1️⃣ Dataset Class & Loaders
- Implemented a PyTorch `Dataset` class to read images and extract labels from filenames.
- Created separate `DataLoader`s for:
  - **Training**
  - **Validation**
  - **Testing**

### 2️⃣ Visualizations
- Plotted class distribution histograms for all three splits.
- Ensured balanced class representation after adjusting splits.

### 3️⃣ Underfitting & Overfitting Scenarios
- Built two CNN models:
  - **Underfitting Model**: Small network with limited capacity
  - **Overfitting Model**: Large network without regularization

### 4️⃣ Loss & Optimization
- Used **CrossEntropyLoss** (suitable for multi-class classification).
- Optimized with **Adam Optimizer** for efficient learning.

### 5️⃣ Training Functions
- `train_one_epoch()` to handle training for one epoch
- `train()` function manages the full training loop, tracks metrics, and prints progress

### 6️⃣ Hyperparameter Tuning
- Used **Weights & Biases (wandb)** to test different learning rates using the validation set
- Selected best learning rate for final training

### 7️⃣ Final Evaluation
- Trained final model on combined training + validation set
- Evaluated accuracy on the **test set**

---

## 🧪 Technologies Used

- **Python 3**
- **PyTorch**
- **torchvision**
- **matplotlib**, **seaborn** – for visualizations
- **wandb** – for experiment tracking and tuning

---

## 🧠 Key Learnings

- Handling image classification with custom datasets
- Designing CNNs that can underfit or overfit to understand model behavior
- Using real-world practices like validation sets and hyperparameter tuning
- Implementing training loops and optimizers manually


