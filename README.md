# 🧮 MNIST Handwritten Digit Recognition using KNN

This project recognizes handwritten digits (0–9) from the MNIST dataset using a **K-Nearest Neighbors (KNN)** machine learning algorithm — *no deep learning used*.

---

## 📂 Project Overview

- Loaded MNIST handwritten digits dataset (train & test CSV)
- Preprocessed and reshaped images (28×28 → 784 features)
- Normalized pixel values using **MinMaxScaler**
- Trained **KNN classifier (k = 3)**
- Evaluated accuracy on validation and test data
- Generated custom handwritten digit using **MS Paint**
- Loaded custom handwritten digit image using **PIL**
- Converted the image to grayscale, resized to **28×28**, flattened & reshaped
- Predicted digit using the trained **KNN model**

---

## 🧠 Algorithm Used

| Component | Details |
|----------|--------|
| Model | K-Nearest Neighbors (KNN) |
| K value | 3 |
| Feature Scaling | MinMaxScaler() |
| Dataset | MNIST (70,000 images) |
| Testing | Custom user-drawn digits & MNIST test data |

---

## 📊 Performance

| Metric | Score |
|--------|------|
| Validation Accuracy | ~ (0.97) |
| Test Accuracy | ~ (0.96) |

> Confusion matrix and classification report generated for detailed analysis.

---

## ✍️ Custom Handwritten Digit Test

- Drew digit using **MS Paint**
- Saved as **.png**
- Loaded image using **PIL**
- Converted to **grayscale** & resized to **28×28**
- Flattened to **(1, 784)** like MNIST format
- Passed to trained **KNN model**
- Model predicted the digit successfully

This simulates **real-world handwritten recognition**.

---

## 📎 Requirements

Install dependencies:

```bash
pip install numpy pandas matplotlib scikit-learn pillow
