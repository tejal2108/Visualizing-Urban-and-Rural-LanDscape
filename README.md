🌆 Visualizing Rural and Urban Landscapes
A machine learning-based system for classifying images into rural or urban categories using BRISK feature descriptors and various supervised classifiers.

📖 Overview
This project presents a machine learning approach to automatically classify images as either rural or urban. By extracting features using the BRISK (Binary Robust Invariant Scalable Keypoints) method and applying supervised learning algorithms such as K-Nearest Neighbors (KNN), Support Vector Machines (SVM), Decision Trees (DT), Random Forests (RF), and Logistic Regression (LR), the system achieves high classification accuracy.

The model has practical applications in areas like disaster relief, land use planning, and environmental monitoring, providing valuable insights for researchers and policymakers.

🗂️ Dataset
Total Images: 2000

Urban: 1000 images

Rural: 1000 images
Each image is resized to 200x200 pixels and converted to grayscale for preprocessing.

🧠 Methodology
Image Preprocessing:

Resize images to 200x200 pixels.

Convert images to grayscale.

Apply Prewitt edge detection.

Feature Extraction:

Use BRISK to extract keypoint descriptors from images.

Clustering:

Apply K-Means clustering to group similar features. Optimal number of clusters (K) determined experimentally.

Classification:

Train and test the following classifiers:

Random Forest (RF)

Decision Tree (DT)

K-Nearest Neighbors (KNN)

Support Vector Machine (SVM)

Logistic Regression (LR)

Evaluation:

Use K-Fold Cross-Validation (K=3) to assess model performance.

Evaluate models based on accuracy, precision, recall, and F1-score.

📊 Results
Classifier	Accuracy	Precision	Recall	F1-Score
Random Forest	99.67%	99.51%	99.83%	99.67%
K-Nearest Neighbors	94.58%	92.92%	96.33%	94.59%
Decision Tree	80.30%	71.32%	87.80%	78.71%
Support Vector Machine	73.20%	70.08%	71.55%	73.78%
Logistic Regression	50.52%	50.81%	96.13%	66.49%

The Random Forest classifier achieved the highest accuracy of 99.67%, indicating its effectiveness for this classification task.

