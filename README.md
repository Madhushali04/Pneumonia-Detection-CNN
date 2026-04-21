# 🫁 Pneumonia Detection from Chest X-Rays using CNN

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=flat-square&logo=python)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?style=flat-square&logo=tensorflow)
![Keras](https://img.shields.io/badge/Keras-Deep%20Learning-red?style=flat-square&logo=keras)
![Streamlit](https://img.shields.io/badge/Streamlit-App-brightgreen?style=flat-square&logo=streamlit)
![License](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)

> A deep learning model that classifies chest X-ray images as **Pneumonia** or **Normal** using a Convolutional Neural Network (CNN), with a Streamlit web interface for real-time predictions.

---

## 📌 Table of Contents

- [About the Project](#about-the-project)
- [Demo](#demo)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Installation & Setup](#installation--setup)
- [How to Run](#how-to-run)
- [Results](#results)
- [What I Learned](#what-i-learned)
- [Future Improvements](#future-improvements)
- [Author](#author)

---

## 🧠 About the Project

Pneumonia is a serious lung infection that affects millions of people worldwide. Early and accurate diagnosis is critical for effective treatment. This project builds an **AI-powered diagnostic tool** that analyzes chest X-ray images and predicts whether a patient has pneumonia or not.

The model is trained on a publicly available Kaggle dataset and achieves high accuracy using a CNN architecture built with TensorFlow and Keras.

---

## 📊 Dataset

- **Source:** [Kaggle - Chest X-Ray Images (Pneumonia)](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)
- **Size:** 5,863 X-Ray images (JPEG)
- **Categories:** 2 classes — `PNEUMONIA` and `NORMAL`
- **Split:**

| Split | Normal | Pneumonia | Total |
|-------|--------|-----------|-------|
| Train | 1,341  | 3,875     | 5,216 |
| Test  | 234    | 390       | 624   |
| Val   | 8      | 8         | 16    |

---

## 🏗️ Model Architecture
Input Layer       → (150, 150, 3) X-ray image
Conv2D + ReLU     → 32 filters, 3x3 kernel
MaxPooling2D      → 2x2 pool size
Conv2D + ReLU     → 64 filters, 3x3 kernel
MaxPooling2D      → 2x2 pool size
Conv2D + ReLU     → 128 filters, 3x3 kernel
MaxPooling2D      → 2x2 pool size
Flatten
Dense + ReLU      → 128 units
Dropout           → 0.5
Dense + Sigmoid   → 1 unit (Binary output)
---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python 3.8+ | Core programming language |
| TensorFlow / Keras | Model building & training |
| NumPy | Numerical operations |
| Matplotlib | Visualization |
| OpenCV | Image preprocessing |
| Kaggle API | Dataset download |

---

## 📈 Results

| Metric | Score |
|--------|-------|
| Training Accuracy | 93.98% |
| Test Accuracy | 87.66% |
| Epochs | 10 |
| Image Size | 150x150 |

---

## 📚 What I Learned

- Building and training a CNN from scratch using TensorFlow/Keras
- Handling class imbalance in medical image datasets
- Applying data augmentation to improve generalization
- Evaluating models using accuracy and loss metrics
- Using Kaggle API to download datasets directly
- Understanding overfitting and dropout layers

---

## 🚀 Future Improvements

- [ ] Use Transfer Learning (VGG16 / ResNet50) for higher accuracy
- [ ] Add Grad-CAM visualization to highlight infected regions
- [ ] Deploy using Streamlit web app
- [ ] Extend to multi-class classification (COVID-19, Tuberculosis)

---

## 👩‍💻 Author

**Madhu**
- 🎓 B.E. in IoT, Cybersecurity & Blockchain 
- 🔗 [LinkedIn](https://www.linkedin.com/in/madhumitha-dhanashekar-9b8245333) | [GitHub](https://github.com/Madhushali04)

---
>  Built with curiosity as part of my AI learning journey!
