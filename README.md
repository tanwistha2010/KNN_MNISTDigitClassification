# KNN Classification Using MNIST Handwritten Digit Dataset

## 1. Project Overview

This project implements a Machine Learning classification model using the **K-Nearest Neighbors (KNN)** algorithm to recognize handwritten digits from 0 to 9.

The project uses the MNIST handwritten digit dataset and Python to train a model that can identify digits from grayscale images.

The implementation is beginner-friendly and performed using Google Colab.

## 2. Objectives

- Understand the K-Nearest Neighbors (KNN) algorithm.
- Load and explore the MNIST dataset.
- Perform data preprocessing and normalization.
- Train a KNN classification model.
- Predict handwritten digits.
- Evaluate model performance using accuracy and other evaluation metrics.

## 3. Dataset Description

The MNIST dataset is a popular dataset used for handwritten digit recognition.

**Dataset Information:**

- Total Images: 70,000
- Original Training Images: 60,000
- Original Testing Images: 10,000
- Image Dimensions: 28 × 28 pixels
- Features per Image: 784
- Image Type: Grayscale
- Classes: 10 (Digits 0–9)

Each image consists of 784 pixel values representing a handwritten digit.

The pixel values range from 0 to 255.

## 4. Algorithm Used: K-Nearest Neighbors (KNN)

KNN is a supervised Machine Learning algorithm used for classification and regression.

It classifies a new data point based on the majority class among its nearest neighbours.

**Working of KNN:**

1. Load the labelled training dataset.
2. Take a new handwritten digit image.
3. Calculate the distance between the new image and training images.
4. Identify the K nearest neighbours.
5. Predict the digit based on majority voting.

In this project, the value of K is set to **3**.

## 5. Technologies and Libraries Used

**Programming Language:** Python

**Platform:** Google Colab

**Libraries:**

- NumPy – For numerical operations.
- Matplotlib – For visualizing handwritten digit images and graphs.
- Scikit-learn – For dataset loading, model creation, training, prediction and evaluation.

## 6. Project Implementation

The project follows these steps:

1. Import the required Python libraries.
2. Load the MNIST dataset using `fetch_openml()`.
3. Separate the image data (X) and labels (y).
4. Visualize sample handwritten digit images.
5. Normalize pixel values between 0 and 1.
6. Split the dataset into training and testing sets.
7. Create a KNN classifier with K = 3.
8. Train the model using the training dataset.
9. Predict handwritten digits using the testing dataset.
10. Evaluate the model performance.

## 7. Data Preprocessing

Before training the model, the pixel values are normalized.

The original pixel values range from 0 to 255.

They are divided by 255 to convert them into a range between 0 and 1.

The dataset is divided into:

- Training Dataset: 10,000 images
- Testing Dataset: 2,000 images

A stratified train-test split is used to maintain the distribution of digit classes.

## 8. Model Evaluation

The KNN model is evaluated using the following metrics:

- **Accuracy:** Measures the percentage of correctly classified images.
- **Precision:** Measures how many predicted class labels are correct.
- **Recall:** Measures how many actual class members are correctly identified.
- **F1-Score:** Combines precision and recall.
- **Confusion Matrix:** Displays the actual and predicted classifications.

The actual evaluation results are generated when the project code is executed.

## 9. Project Structure

```text
KNN-MNIST-Classification/
│
├── knn_mnist.ipynb
├── README.md
└── requirements.txt
```

## 10. Installation and Execution

Install the required libraries:

```bash
pip install numpy matplotlib scikit-learn
```

**Steps to run the project:**

1. Open Google Colab.
2. Create a new notebook.
3. Copy the project code into separate cells.
4. Execute the cells in the correct order.
5. Wait for the MNIST dataset to load.
6. View the predictions and evaluation results.

Dataset downloading requires an internet connection.

## 11. Advantages of KNN

- Simple and easy to understand.
- Easy to implement.
- Supports multi-class classification.
- Does not require a complex model training process.

## 12. Limitations

- Prediction can be slow for large datasets.
- Requires storing the training data.
- Performance depends on the choice of K.
- Can be affected by irrelevant features and noisy data.

## 13. Future Scope

- Use the complete MNIST dataset for experimentation.
- Compare KNN with other classification algorithms such as SVM and CNN.
- Improve prediction efficiency.
- Develop a web application for handwritten digit recognition.

## 14. Conclusion

This project demonstrates how the K-Nearest Neighbors algorithm can be used for handwritten digit classification using the MNIST dataset.

Through this project, we understand the basic concepts of supervised Machine Learning, data preprocessing, normalization, model training, prediction and performance evaluation.

It provides a practical introduction to image classification using Python and Scikit-learn.

---

*Developed as a beginner-friendly Machine Learning academic project.*
