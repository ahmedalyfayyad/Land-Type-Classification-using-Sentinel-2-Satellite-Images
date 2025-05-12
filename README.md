# 🌍 Land Type Classification using Sentinel-2 Satellite Images

This project aims to classify land types using Sentinel-2 multispectral satellite images and deep learning. It supports real-time predictions via a deployed model and allows users to upload images and visualize classified results on a map.

## 🛰️ Project Overview

- **Dataset**: [EuroSAT-MS (13-band)](https://github.com/phelber/eurosat) based on Sentinel-2 imagery.
- **Classes**: Agriculture, Water, Urban, Desert, Roads, Trees.
- **Model**: Custom ResNet18 adapted for 13 spectral bands.
- **Deployment**: Flask API hosted on Azure for real-time inference.
- **Visualization**: Classified image preview and per-class accuracy statistics.

---

## ⚙️ Features

- Preprocessing and normalization of 13-band .tif satellite images.
- 5-fold cross-validation and performance metrics (accuracy, F1-score, confusion matrix).
- Hyperparameter tuning, model refinement (BatchNorm, EarlyStopping).
- User-friendly interface for uploading satellite images (.tif, .jpg, etc.).
- Interactive map and plots (Matplotlib/Plotly) for visualizing predictions.

---

## 🧠 Model Training

- Implemented using PyTorch.
- Dataset split into training, validation, and test sets.
- Normalization based on dataset-wide band mean and standard deviation.
- Performance tuned with learning rate, batch size, dropout, and architecture depth.

---

## 🚀 Deployment

- Real-time predictions via Azure-hosted Flask API.
- Accepts image uploads (TIFF, JPG, PNG).
- Outputs predicted land class with visual overlay.

---

## 🖼️ Visualization

- Color-coded land type predictions.
- Statistics of class-wise prediction accuracy on the map of Egypt.
- Bar charts and confusion matrices for model interpretability.

---

## 💻 How to Use

1. Clone this repository:
   ```bash
   git clone https://github.com/your-friend-username/your-repo-name.git
   cd your-repo-name
