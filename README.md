# 🖼️ MNIST Image Classification with Custom CNN

## 📌 Project Overview
This project implements an image classification pipeline on the **MNIST dataset** using a Convolutional Neural Network (CNN). The MNIST dataset contains 28x28 grayscale images of handwritten digits (0-9). The CNN architecture includes multiple convolutional layers for feature extraction and dense layers for classification. The goal is to classify the digits accurately by utilizing modern CNN techniques.

---

## 🎯 Objective
Classify images from the [MNIST dataset](http://yann.lecun.com/exdb/mnist/) that consist of 28x28 pixel grayscale images of handwritten digits. The project demonstrates the development of a custom CNN model for image classification.

---

## 💡 Why This Project?
This project was built to:
- Explore and understand Convolutional Neural Networks (CNNs) for image classification.
- Implement basic image classification using the MNIST dataset, showcasing practical usage of CNNs.

---

## 🔑 Key Steps

### 📦 1. Importing Required Libraries
- `TensorFlow/Keras` — used for model building and training
- `NumPy` — used for array manipulation
- `Matplotlib` — used for visualizing training and validation metrics

---

### 🗂️ 2. Dataset Loading & Splitting
- The MNIST dataset is loaded directly from `tf.keras.datasets`.
- The dataset is split into **training** (60,000 samples) and **test** (10,000 samples).

---

### 🧼 3. Preprocessing
- **Normalization:** Pixel values are normalized to a range between 0 and 1 for better model performance.
- **Reshaping:** The images are reshaped to fit the input layer of the CNN (28x28x1).

---

### 🧪 4. Custom CNN Model Architecture
A custom CNN was created using:
- Multiple `Conv2D` layers for feature extraction
- `MaxPooling2D` layers to reduce spatial dimensions
- `Dense` layers for classification
- Regularization techniques such as **Dropout** and **BatchNormalization** to avoid overfitting

The architecture includes:
- 3 convolutional layers with increasing filter sizes
- 2 dense layers for classification
- A softmax output layer with 10 neurons (one for each class: 0-9)

---

### 🚀 5. Model Compilation & Training
- The model is compiled with:
  - **Loss function:** `sparse_categorical_crossentropy`
  - **Optimizer:** `Adam`
  - **Metrics:** `accuracy`
- The model is trained for **15 epochs** with a batch size of **32**, and training performance is monitored on both training and validation datasets.

---

### 📊 6. Performance Monitoring
- The training and validation accuracy are monitored to evaluate the model's ability to generalize to unseen data.
- The model is evaluated on the test set to check its final performance.

---

### 🏆 7. Results
The model achieved an **accuracy of around 98%** on the validation set after 15 epochs of training. This is a strong result, demonstrating that the custom CNN model is capable of recognizing handwritten digits effectively.

---

## 📈 Model Performance

| **Model Type**   | **Test Accuracy** | **Test Loss** |
|------------------|-------------------|---------------|
| Custom CNN      | **98.0%**          | 0.0344        |

---

## 📁 Files Included
- 📓 [MNIST_CNN_Model.ipynb](./MNIST_CNN_Model.ipynb)
- 📦 [MNIST Dataset](https://www.kaggle.com/oddrationale/mnist-in-csv) or direct import from TensorFlow

---

## 💡 Recommendations for Further Improvement

Here are a few ways this project can be extended and improved:

1. **Experiment with Advanced Architectures**  
   Try more complex architectures like ResNet or VGG for higher performance.

2. **Implement Data Augmentation**  
   Use data augmentation techniques like rotation, scaling, or flipping to improve generalization and reduce overfitting.

3. **Hyperparameter Tuning**  
   Experiment with different hyperparameters like learning rate, batch size, and filter sizes to optimize model performance.

---

## 📦 Requirements
- `TensorFlow: 2.x`
- `Keras: 2.x`
- `NumPy: 1.18.x`
- `Matplotlib: 3.3.x`

---

## 🧠 Author Note
Feel free to explore and experiment with this project! For any questions or suggestions, don’t hesitate to reach out.
