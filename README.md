# 📷 Sign Language Recognition Using Machine Learning

This project explores the application of various machine learning and deep learning algorithms to recognize American Sign Language (ASL) letters. The goal is to identify effective, resource-conscious methods for sign language recognition, contributing to the development of assistive technologies for the mute and hard of hearing.

---

## 💾 Dataset

The project utilizes the **Sign Language MNIST dataset**.

* **Source:** Downloaded directly from Kaggle.
* **Files Used:** `sign_mnist_train.csv` and `sign_mnist_test.csv`.
* **Data Structure:** The training data consists of 27,455 entries and 785 columns. The columns include a `label` (the ASL letter) and 784 pixel columns (`pixel1` to `pixel784`) representing the image data.

---

## 🛠️ Methodology and Workflow

The entire workflow, from data preparation to model evaluation, is contained within the `Sign Language Recognition.ipynb` Jupyter Notebook.

### Key Steps:

1.  **Data Acquisition:** Downloading and reading the Sign Language MNIST dataset.
2.  **Data Preparation:** Performing the Train/Test split and basic Data Exploration (EDA).
3.  **Preprocessing:** Data Preprocessing steps, including scaling and reshaping the pixel data.
4.  **Data Augmentation:** Using `ImageDataGenerator` (from Keras) to expand the training set and improve model generalization.
5.  **Model Fitting and Training:** Evaluation of multiple models for classification.

### Models Evaluated

The project rigorously evaluated both classic Machine Learning and Deep Learning approaches:

* **Support Vector Machine (SVM)**
* **k-Nearest Neighbors (K-NN)**
* **Random Forests**
* **Convolutional Neural Network (CNN)**

---

## 📈 Results

The models demonstrated strong performance in classifying the ASL letters:

* **Random Forest Classifier:** Achieved an **accuracy of 94%** on the test set.
* **Convolutional Neural Network (CNN):** Showed consistent accuracy improvement over 15 epochs, reaching a final training accuracy of **~97.05%**.
* **Evaluation:** Comprehensive evaluation was conducted using a classification report and confusion matrices for the models tested.
