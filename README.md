# 😷 Face Mask Detection using Transfer Learning (VGG16)



This project is a **Face Mask Detection System** built with **Transfer Learning** using the **VGG16 architecture**.  
The model classifies whether a person is wearing a mask or not. It also supports **live webcam predictions** via Google Colab’s JavaScript integration.

---

## 🚀 Tech Stack  

![Python](https://img.shields.io/badge/Language-Python-blue?logo=python)  
![Colab](https://img.shields.io/badge/Platform-Google%20Colab-orange?logo=googlecolab&logoColor=white)  
![Keras](https://img.shields.io/badge/Library-Keras-red?logo=keras)  
![TensorFlow](https://img.shields.io/badge/Framework-TensorFlow-orange?logo=tensorflow)  
![OpenCV](https://img.shields.io/badge/Library-OpenCV-green?logo=opencv)  
![scikit-learn](https://img.shields.io/badge/Library-Scikit--Learn-F7931E?logo=scikit-learn&logoColor=white)  
![NumPy](https://img.shields.io/badge/Library-NumPy-013243?logo=numpy)  
![Pandas](https://img.shields.io/badge/Library-Pandas-150458?logo=pandas)  

---

## 📌 Project Overview

This was a fun project that helped me build strong fundamentals in **Computer Vision** and **Deep Learning**.  

Key steps I implemented:
- 📂 Loading and organizing image data from Google Drive  
- 📝 Reading metadata from a CSV file with **pandas**  
- 🖼️ Preprocessing images using **OpenCV** (resizing, normalization, and conversion)  
- 🔀 Shuffling and splitting dataset using **scikit-learn**  
- 🧠 Building a **Transfer Learning model** with **VGG16** from `keras.applications`  
- ❄️ Freezing convolutional base and adding a **custom head** for binary classification  
- 📊 Training and evaluating the model  
- 📸 Live prediction using Colab webcam (with a **JavaScript workaround** since `cv2.imshow` doesn’t work in Colab)  
- 🌐 Testing predictions on internet sample images  

---

## 🚀 Features

- ✅ **Binary classification**: Mask 😷 / No Mask 🙂  
- ✅ **Transfer Learning** using VGG16  
- ✅ **Live prediction** using Colab webcam  
- ✅ **End-to-End pipeline**: data loading → preprocessing → training → evaluation → deployment  

---


## 📂 Dataset

- The dataset consisted of **1279 images** stored in two categories:
  - `with_mask`
  - `without_mask`  
- A metadata file `_classes.csv` contained labels for each image.

---

## 📸 Live Webcam Prediction (in Colab)

Since **`cv2.imshow` doesn’t work in Colab**, I used a **JavaScript bridge** to capture webcam frames and feed them to the trained model for prediction:

- **1 → With Mask 😷**  
- **0 → Without Mask 🙂**

---

## ⚙️ Model Architecture

- **Base Model**: VGG16 (pretrained on ImageNet)  
- **Frozen layers**: Convolutional base  
- **Custom Head**: Dense layers for binary classification  

---

## 📊 Results  

- **Training Accuracy:** `0.9348`  
- **Training Loss:** `0.2387`  
- **Validation Accuracy:** `0.9570`  
- **Validation Loss:** `0.1922`  

---

## 💡 Learnings

This project strengthened my understanding of:
- Loading and preprocessing image data  
- Building custom pipelines in Colab  
- Transfer Learning concepts  
- Handling Colab environment limitations with creative workarounds  
- End-to-end Computer Vision project structure  

---

## 🚀 Future Work

- Add **data augmentation** for more robust training  
- Experiment with **lighter models** (MobileNetV2, EfficientNet) for faster inference  
- Add **Grad-CAM visualizations** to interpret model predictions  
- Deploy as a **web app** using Streamlit or Flask  

---

## 🙌 Acknowledgments

Thanks to **Keras, TensorFlow, and Colab** for making this project possible ✨  

---

