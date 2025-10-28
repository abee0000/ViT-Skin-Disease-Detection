<h1 align="center">🧠 Skin Disease Detection Based on Vision Transformer (ViT)</h1>

<p align="center">
  <strong>AI-Powered Dermatology: Leveraging Vision Transformers for Accurate Skin Disease Diagnosis</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10-blue?logo=python" />
  <img src="https://img.shields.io/badge/TensorFlow-2.17-orange?logo=tensorflow" />
  <img src="https://img.shields.io/badge/Transformers-HuggingFace-yellow?logo=huggingface" />
  <img src="https://img.shields.io/badge/License-MIT-green" />
</p>

---

## Overview
Skin diseases affect millions globally, and early detection plays a crucial role in preventing severe complications.  
This project introduces a **deep learning-based diagnostic system** using **Vision Transformers (ViT)** — a state-of-the-art model architecture renowned for its ability to understand global image dependencies better than traditional Convolutional Neural Networks (CNNs).

Through extensive experimentation, we developed, trained, and deployed a Vision Transformer model capable of classifying **four major skin conditions** with **91.19% test accuracy**.

---

##  Key Highlights
- **90%+ classification accuracy** using ViT-B/16 architecture  
- **Comparison between CNN and ViT models**  
- **Desktop application with Tkinter** for real-time disease classification  
- **Confidence score visualization** for user interpretability  
- **Dataset of 8,000 labeled dermoscopic images**  

---

## Project Architecture

### Workflow

### Vision Transformer Pipeline
1. **Image Tokenization:** Split input image into 16×16 patches  
2. **Linear Embedding:** Flatten and embed patches into 1D tokens  
3. **Positional Encoding:** Retain spatial structure  
4. **Self-Attention:** Each patch attends to all others for global context  
5. **Classification Head:** Final layer predicts disease category  

---

## Repository Structure

---

## Tech Stack

| Category | Tools Used |
|-----------|-------------|
| Programming Language | Python 3.10+ |
| Frameworks | TensorFlow, HuggingFace Transformers |
| ML Libraries | Scikit-learn, NumPy, Pandas |
| Visualization | Matplotlib, Seaborn |
| GUI | Tkinter, tkinterDnD2 |
| Environment | Jupyter Notebook / VSCode |
| OS | Windows / Linux / macOS |

---

## Model Summary

| Model | Accuracy | F1-Score | AUC |
|--------|-----------|----------|------|
| CNN (Benchmark) | 78.3% | 77% | 0.88 |
| ViT-B16 | **91.19%** | **90%+** | **0.99** |

**ROC-AUC by Class:**
- **Basal Cell Carcinoma (BCC):** 0.99  
- **Benign Keratosis (BKL):** 0.96  
- **Melanoma (MEL):** 1.00  
- **Melanocytic Nevi (NV):** 0.99  

---

## Visual Results

### Accuracy vs Loss
![Accuracy and Loss Curve](./results/accuracy_loss_curves.png)

### Confusion Matrix
![Confusion Matrix](./results/confusion_matrix.png)

### ROC Curves
![ROC Curve](./results/roc_curve.png)

---

## How to Run the Application

### 1️Clone the Repository
```bash
git clone https://github.com/<your-username>/skin-disease-detection-vit.git
cd skin-disease-detection-vit
pip install -r requirements.txt
cd app
python main.py


