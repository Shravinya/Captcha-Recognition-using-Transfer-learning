
# 🧠 CAPTCHA Recognition using CRNN + CTC Loss

> An end-to-end deep learning model to decode distorted CAPTCHA text images using **Convolutional Recurrent Neural Networks (CRNN)** and **Connectionist Temporal Classification (CTC) Loss**.

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![TensorFlow](https://img.shields.io/badge/TensorFlow-orange?logo=tensorflow)
![PyTorch](https://img.shields.io/badge/PyTorch-red?logo=pytorch)
![OpenCV](https://img.shields.io/badge/OpenCV-blue?logo=opencv)
![DeepLearning](https://img.shields.io/badge/Deep%20Learning-Enabled-green)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

## 📋 Project Overview

CAPTCHAs (Completely Automated Public Turing tests to tell Computers and Humans Apart) are designed to differentiate humans from bots.  
This project builds an **intelligent OCR system** that can accurately recognize distorted CAPTCHA images without explicit segmentation or alignment.

The proposed model integrates:
- 🧩 **CNNs** for spatial feature extraction  
- 🔁 **BiLSTMs** for sequence modeling  
- 🧠 **CTC Loss** for alignment-free decoding  

---

## 🎯 Objectives

- Develop a robust **end-to-end CAPTCHA recognition pipeline**.  
- Handle **variable-length sequences**, distortions, and noise.  
- Achieve high accuracy through **hybrid CRNN architecture**.  
- Demonstrate real-world applicability across OCR and automation systems.

---

## 🏗️ System Architecture

```mermaid
graph TD
A[Input CAPTCHA Image] --> B[Data Preprocessing]
B --> C[CNN: Feature Extraction]
C --> D[BiLSTM: Sequence Modeling]
D --> E[CTC Decoder: Alignment-free Text Prediction]
E --> F[Predicted CAPTCHA Text]
