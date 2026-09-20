# Pneumonia Detection

A deep learning model for detecting pneumonia from chest X-ray images, classifying them into 3 categories, built as part of the MedScan graduation project.

🔗 Part of: [MedScan — AI-Powered Medical Image Analysis Platform](https://github.com/kholoiud-Mohammed-Zaki22/MedScan)

## 📌 Overview
This model classifies chest X-ray images into 3 categories using transfer learning with EfficientNetB0. It is deployed as an independent FastAPI service, containerized with Docker, and hosted on Railway.

## 📊 Dataset
- Source: [Kaggle](https://www.kaggle.com)
- 3-class chest X-ray pneumonia dataset

## 🧠 Model
- Architecture: EfficientNetB0 (Transfer Learning)
  - 238 layers total, first 100 layers frozen
- Framework: TensorFlow 2.19 / Keras
- Preprocessing note: No /255 normalization applied — EfficientNetB0 handles normalization internally
- Accuracy: ~95–99% on the test set

## 🚀 Deployment
- Served via FastAPI as a REST API
- Containerized with Docker
- Deployed on Railway, with dynamic PORT binding
- Model weights hosted on Google Drive and loaded at startup via gdown

## 🛠️ Tech Stack
Python · TensorFlow · Keras · FastAPI · Docker · Railway

## 👥 Team
Developed as part of the MedScan graduation project, supervised by Dr. Abdulla M. Hassan, with teammates Gehad Abdelrady Mostafa and Toqa Usama Mohamed.
