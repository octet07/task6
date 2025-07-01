# Iris Dataset Classification with KNN

This project performs classification on the Iris dataset using the K-Nearest Neighbors (KNN) algorithm. The workflow includes loading and preprocessing the data, normalizing features, experimenting with different values of K, evaluating model performance, and visualizing decision boundaries.

## 1. Dataset and Normalization

The Iris dataset consists of four numerical features: SepalLengthCm, SepalWidthCm, PetalLengthCm, and PetalWidthCm, with the target variable being Species (Setosa, Versicolor, Virginica). We loaded the dataset and separated the features (X) and target (y). To ensure uniform feature scaling, we applied standard normalization using `StandardScaler` from scikit-learn.

## 2. Train/Test Split and Model Training

The dataset was split into training and testing sets using an 80-20 ratio. We then initialized and trained a `KNeighborsClassifier` with k=5 using the training data. The model was used to predict the labels for the test set, and the accuracy was calculated.

## 3. Experimenting with Different K Values

To understand how the value of K affects model performance, we evaluated the classifier for K values ranging from 1 to 15. For each K, the model was trained and tested, and the corresponding accuracy was recorded. The results were visualized in a plot showing accuracy versus K.

## 4. Model Evaluation with Accuracy and Confusion Matrix

The performance of the KNN classifier (k=5) was evaluated using accuracy and a confusion matrix. The confusion matrix visually represents the classifier's ability to correctly predict the classes, and provides insight into misclassifications.

## 5. Visualizing Decision Boundaries

To visualize how the KNN classifier separates classes, we plotted decision boundaries using the first two normalized features (SepalLengthCm and SepalWidthCm). A meshgrid was created to cover the feature space, predictions were made over the grid, and the boundaries were visualized along with the actual data points. This provided an intuitive understanding of the model's decision regions.

---
