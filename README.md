# 📘 Deep Learning: Wine Quality Prediction

## 🧠 Project Overview

This project involves training dense neural networks for both binary and multi-class classification on the Wine Quality dataset. It also includes a comparison with traditional machine learning approaches to evaluate the effectiveness of deep learning models.

---

## 📂 Dataset Description

- **Source**: [UCI Wine Quality Dataset](https://archive.ics.uci.edu/ml/datasets/wine+quality)  
- **Samples**: 1,599  
- **Features**: 11 numerical features (e.g., fixed acidity, volatile acidity, citric acid, etc.)  
- **Target Variable**: `quality`  
  - **Binary Classification**: `good` (≥ 7) vs. `bad` (< 7)  
  - **Multi-Class Classification**:

| Label       | Quality Score Range |
|-------------|---------------------|
| 0 (Bad)     | ≤ 4                 |
| 1 (Medium)  | 5–6                 |
| 2 (Good)    | ≥ 7                 |

---

## 🏗️ Modeling Approaches

| Task                    | Model                        | Output             | Configuration                                              |
|-------------------------|------------------------------|--------------------|-----------------------------------------------------------|
| Binary Classification   | Keras Neural Network         | 0 (bad) / 1 (good) | 2 dense layers, 128 units/layer, Adam optimizer, 400 epochs |
| Multi-Class Classification | Keras Neural Network      | 0, 1, 2            | Same as above                                             |
| Benchmarking            | `MLPClassifier` (Scikit-learn) | 0, 1, 2          | Default MLP training settings                             |

---

## 📈 Evaluation Metrics

- Training & validation loss  
- Final test loss and accuracy  
- Confusion matrix and classification reports  
- Comparison between Keras and Scikit-learn models  

---

## ⚠️ Known Issues and Feedback

### 🔴 Issues to Address

1. **Model Retraining Omission**  
   In Section 6, the retraining of the model after introducing new hyperparameters or data preprocessing steps was missing. Retraining is necessary to ensure the changes take effect in the final evaluation.

2. **Incomplete Answer**  
   While the explanation in Section 8 is factually correct, it could benefit from a more comprehensive discussion—such as an analysis of model interpretability, implications of class imbalance, or tuning methods used for optimization.

---

> 📌 *Note: Contributions and suggestions are welcome. Please feel free to open issues or submit pull requests to improve this project.*

