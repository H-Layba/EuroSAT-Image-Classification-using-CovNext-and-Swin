# EuroSAT-Image-Classification-using-CovNext-and-Swin

This project focuses on **multi-class land use classification** using the EuroSAT dataset. It compares two advanced deep learning architectures — **ConvNeXt** and **Swin Transformer** — for satellite image classification.

---

##  Project Overview

- Built a complete deep learning pipeline for image classification
- Compared CNN-based (ConvNeXt) and Transformer-based (Swin) architectures
- Evaluated models using comprehensive classification metrics
- Performed dataset preprocessing, splitting, training, and inference
- Tested models on real-world images for practical validation

---

##  Dataset

- **Dataset:** EuroSAT (Satellite Image Classification Dataset)
- **Classes (10):**
  - AnnualCrop  
  - Forest  
  - HerbaceousVegetation  
  - Highway  
  - Industrial  
  - Pasture  
  - PermanentCrop  
  - Residential  
  - River  
  - SeaLake  

---

##  Data Preprocessing

- Mounted Google Drive for dataset access
- Cleaned and validated dataset folders
- Split dataset into:
  - 70% Training
  - 15% Validation
  - 15% Testing
- Applied image transformations:
  - Resize (224×224)
  - Normalization (ImageNet stats)
  - Data augmentation (rotation, flipping, color jitter)

---

##  Models Used

###  ConvNeXt Base
- Pretrained on ImageNet
- Fine-tuned for EuroSAT dataset
- Used cross-entropy loss
- Optimized for high accuracy classification

###  Swin Transformer Base
- Vision Transformer architecture
- Window-based self-attention mechanism
- Pretrained + fine-tuned on dataset
- Strong performance on spatial feature learning

---

##  Training Pipeline

- Optimizer: AdamW
- Loss Function: CrossEntropyLoss
- Batch Size: 16–32
- Epochs: 5+
- Frameworks: PyTorch, timm, torchvision

---

##  Evaluation Metrics

The following metrics were used for performance evaluation:

- Accuracy
- Balanced Accuracy
- Precision (Macro, Micro, Weighted)
- Recall (Macro, Micro, Weighted)
- F1 Score (Macro, Micro, Weighted)
- Matthews Correlation Coefficient (MCC)
- Cohen’s Kappa Score
- Cross Entropy Loss

---

##  Results Summary

| Model        | Accuracy | F1 Score (Macro) | MCC   |
|--------------|----------|------------------|--------|
| ConvNeXt     | ~97.5%   | ~0.974           | ~0.972 |
| Swin Transformer | ~97.7% | ~0.977         | ~0.975 |

 Swin Transformer slightly outperformed ConvNeXt in overall performance.

---

##  Visual Analysis

The project includes:

- Training vs Validation Accuracy/Loss graphs
- Per-class Precision, Recall, F1-score comparison
- Confusion matrices
- Model performance comparison charts
- Real image prediction visualizations

---

##  Inference / Prediction

Both models support real-time prediction:

- Upload an image
- Preprocess using trained pipeline
- Get predicted land-use class
- Display class probabilities

---

##  Key Features

- End-to-end deep learning pipeline
- CNN vs Transformer comparison
- Real-world satellite image classification
- Detailed evaluation metrics
- Visualization of model performance
- Google Drive integration for large datasets

---

##  Tech Stack

- Python
- PyTorch
- Torchvision
- timm (pretrained models)
- Scikit-learn
- Matplotlib & Seaborn
- Google Colab

---

##  Project Highlights

- Built and trained **ConvNeXt + Swin Transformer models**
- Achieved **state-of-the-art accuracy on EuroSAT dataset**
- Performed **multi-metric evaluation (not just accuracy)**
- Implemented **real-world inference system**
- Compared **CNN vs Transformer performance**

---

## 📁 Folder Structure
