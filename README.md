# 🍎🥦 Fruit & Vegetable Recognition System

## 📌 Project Description

This is a simple and interactive web application that allows users to upload an image of a fruit or vegetable.  
The system automatically classifies the image using artificial intelligence and displays the predicted name along with a visual emoji animation for an engaging experience.  
The project leverages deep learning and computer vision techniques for accurate classification.

---

## 🛠️ Tools & Libraries Used

- **TensorFlow / Keras**  
  Used for deep learning tasks, especially for feature extraction using DenseNet121.

- **Adaptive Particle Grey Wolf Optimization (APGWO)**  
  Applied for feature selection to optimize performance and reduce dimensionality.

- **Scikit-learn**  
  Utilized to train classical machine learning models including:
  - K-Nearest Neighbors (KNN)
  - Decision Tree
  - Support Vector Machine (SVM)
  - Random Forest
  - Multi-layer Perceptron (MLP)

- **Joblib**  
  For saving and loading the trained models efficiently.

- **NumPy**  
  For handling image arrays and feature vectors.

- **Pillow**  
  Used to process and manipulate images.

- **Streamlit**  
  Provides a simple and fast way to build and deploy the web application.

---

## 🧠 How It Works

1. The user uploads an image file (`.jpg`, `.png`, or `.jpeg`).
2. The image is resized to 224x224 pixels.
3. **DenseNet121** extracts deep features from the image.
4. **APGWO** selects the most relevant features.
5. A pre-trained classifier predicts the class of the image.
6. The predicted label and a falling emoji effect are displayed on the interface.

---

## 📊 Dataset Information

- **Dataset Name:** Fruit360  
- **Source:** [Fruit360 on Kaggle](https://www.kaggle.com/moltean/fruits)  
- **Total Images:** 90,000+  
- **Image Size:** 100x100  
- **Number of Classes in Dataset:** 131  
- **Classes Used in This Application:**
  - Apple 🍎
  - Cabbage 🥬
  - Carrot 🥕
  - Zucchini 🥒
  - Pear 🍐
  - Cucumber 🥒

---

## 🚀 Deployment

This application is built with **Streamlit** and can be run locally using the following command:

```bash
streamlit run fruit.py
