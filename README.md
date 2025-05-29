# 🌆 Visualizing Rural and Urban Landscapes

*A machine learning-based system for classifying images into rural or urban categories using BRISK feature descriptors and various supervised classifiers.*

---

## 📖 Overview

This project presents a machine learning approach to automatically classify images as either **rural** or **urban**. By extracting features using the **BRISK (Binary Robust Invariant Scalable Keypoints)** method and applying supervised learning algorithms such as:

* K-Nearest Neighbors (KNN)
* Support Vector Machines (SVM)
* Decision Trees (DT)
* Random Forests (RF)
* Logistic Regression (LR)

the system achieves **high classification accuracy**.

---

## 🗂️ Dataset

* **Total Images**: 2000

  * **Urban**: 1000 images
  * **Rural**: 1000 images

Each image is:

* Resized to **200x200 pixels**
* Converted to **grayscale** for preprocessing

---

## 🧠 Methodology

### 1. Image Preprocessing

* Resize images to 200x200 pixels
* Convert to grayscale
* Apply **Prewitt edge detection**

### 2. Feature Extraction

* Use **BRISK** to extract keypoint descriptors

### 3. Clustering

* Use **K-Means** to cluster similar features
* Optimal `K` selected experimentally

### 4. Classification

Train and test the following classifiers:

* Random Forest (RF)
* Decision Tree (DT)
* K-Nearest Neighbors (KNN)
* Support Vector Machine (SVM)
* Logistic Regression (LR)

### 5. Evaluation

* Use **K-Fold Cross-Validation** (K = 3)
* Evaluate with:

  * Accuracy
  * Precision
  * Recall
  * F1-score

---

## 📊 Results

| Classifier                 | Accuracy | Precision | Recall | F1-Score |
| -------------------------- | -------- | --------- | ------ | -------- |
| **Random Forest**          | 99.67%   | 99.51%    | 99.83% | 99.67%   |
| **K-Nearest Neighbors**    | 94.58%   | 92.92%    | 96.33% | 94.59%   |
| **Decision Tree**          | 80.30%   | 71.32%    | 87.80% | 78.71%   |
| **Support Vector Machine** | 73.20%   | 70.08%    | 71.55% | 73.78%   |
| **Logistic Regression**    | 50.52%   | 50.81%    | 96.13% | 66.49%   |

> ✅ The **Random Forest** classifier achieved the **highest accuracy (99.67%)**, demonstrating its effectiveness for this classification task.

---
