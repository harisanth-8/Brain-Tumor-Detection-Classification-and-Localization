# 🧠 Brain Tumor Detection, Classification and Localization using Random Forest & SVM

A Machine Learning-based Brain Tumor Detection System developed using **Random Forest (RF)** and **Support Vector Machine (SVM)** for binary tumor detection, multi-class tumor classification, and approximate tumor localization from MRI images.

> **Project Domain:** Medical Image Processing | Machine Learning | Computer Vision

---

## 📌 Project Overview

Brain tumor diagnosis from MRI images is a challenging and time-consuming task. This project aims to assist medical professionals by automatically detecting the presence of a brain tumor, classifying the tumor type, and providing an approximate localization of the tumor region.

Unlike deep learning approaches, this project utilizes **classical machine learning algorithms** with handcrafted image features for efficient and computationally lightweight prediction.

---

## 🎯 Objectives

- Detect whether an MRI scan contains a brain tumor.
- Classify the detected tumor into one of the predefined classes.
- Perform approximate tumor localization using Region of Interest (ROI).
- Evaluate the performance using standard machine learning metrics.

---

## 🧩 Project Modules

### Module 1 – Data Acquisition & Preparation
- Download MRI dataset
- Image preprocessing
- Grayscale conversion
- Image resizing (128 × 128)
- Pixel normalization
- Dataset splitting

---

### Module 2 – Feature Extraction

Feature extraction is performed using:

- Histogram of Oriented Gradients (HOG)
- Raw Pixel Features

The extracted features are combined to improve classification performance.

---

### Module 3 – Tumor Detection (Binary Classification)

Models Used:

- Random Forest
- Support Vector Machine (SVM)

Output:

- Tumor
- No Tumor

---

### Module 4 – Tumor Classification (Multi-Class)

Classifies MRI images into:

- Glioma
- Meningioma
- Pituitary Tumor
- No Tumor

Models Used:

- Random Forest
- Support Vector Machine (SVM)

---

### Module 5 – Tumor Localization

Since Random Forest and SVM cannot perform spatial localization, an approximate localization technique is implemented.

Localization is performed using a **knowledge-guided Region of Interest (ROI)** approach based on the predicted tumor class.

| Tumor Type | Approximate ROI |
|------------|----------------|
| Glioma | Central Region |
| Meningioma | Upper/Edge Region |
| Pituitary | Center-Bottom Region |
| No Tumor | No Bounding Box |

---

### Module 6 – Final Prediction

The system supports prediction on:

- Images from the dataset
- External MRI images

Output includes:

- Tumor Detection
- Tumor Classification
- Tumor Localization

---

# 🗂 Dataset

Dataset Used:

**Brain Tumor MRI Dataset**

Classes:

- Glioma
- Meningioma
- Pituitary
- No Tumor

Source:
https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset

---

# ⚙️ Technologies Used

- Python
- OpenCV
- NumPy
- Matplotlib
- Scikit-learn
- scikit-image
- Kaggle API

---

# 🧠 Machine Learning Models

### Binary Detection

- Random Forest Classifier
- Support Vector Machine (RBF Kernel)

---

### Multi-Class Classification

- Random Forest Classifier
- Support Vector Machine (RBF Kernel)

---

# 🔍 Feature Engineering

Features extracted:

- Histogram of Oriented Gradients (HOG)
- Raw Pixel Intensities

Feature Scaling:

- StandardScaler

---

# 📊 Evaluation Metrics

The models are evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Classification Report

---

# 📁 Project Structure

```
Brain-Tumor-Detection/
│
├── data/
│   ├── Training/
│   └── Testing/
│
├── Brain_Tumor_Detection.ipynb
├── README.md
└── requirements.txt
```

---

# 🚀 Workflow

```
MRI Image
      │
      ▼
Image Preprocessing
      │
      ▼
Feature Extraction
(HOG + Raw Pixels)
      │
      ▼
Feature Scaling
      │
      ▼
Tumor Detection
(Random Forest / SVM)
      │
      ▼
Tumor Classification
(Random Forest / SVM)
      │
      ▼
ROI-Based Localization
      │
      ▼
Final Prediction
```

---

# 📸 Sample Output

The system provides:

- MRI Image Display
- Tumor Detection Result
- Predicted Tumor Type
- Approximate Tumor Localization using Bounding Box

---

# 📈 Future Enhancements

- CNN-based Feature Learning
- YOLO-based Precise Tumor Localization
- U-Net Tumor Segmentation
- Model Deployment using Flask or Streamlit
- Explainable AI (Grad-CAM)
- Clinical Decision Support Integration

---

# 👨‍💻 Authors

Developed as an academic Machine Learning project focusing on Brain Tumor Detection, Classification, and Localization using Random Forest and Support Vector Machine.

---

# 📄 License

This project is developed for educational and research purposes.
