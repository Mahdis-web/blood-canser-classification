"
# 🩸 Acute Lymphoblastic Leukemia (ALL) Subtype Classification (L1, L2, L3)

This project focuses on classifying acute lymphoblastic leukemia (ALL) into its three subtypes (L1, L2, L3) using deep learning techniques on real-world medical data.


## 📌 Project Overview

- *Goal:* Detect and classify ALL subtypes from microscopic blood cell images
- *Dataset:* Real stained blood smear images, collected and labeled by a pathologist
- *Scope:* End-to-end deep learning pipeline — from raw data to subtype classification


## 🧪 Dataset Description

- High-resolution microscopic images of stained blood cells
- Initially multi-cellular; later cropped into *single-cell images*
- Expert-annotated into five classes:
  - *Normal*
  - *Blast*
  - *L1, **L2, **L3*

> ✅ Images were used *without preprocessing* to test model robustness on real, noisy data.


## 🧠 Models & Techniques

- *CNN* for initial feature extraction
- *Transfer Learning & Fine-Tuning* using:
  - VGG
  - ResNet
  - DenseNet
  - InceptionV3
  - Xception


## ✨ Innovation & Learning Strategy

This project introduces a hybrid deep learning pipeline that combines multiple advanced strategies to achieve strong performance without traditional preprocessing:

- 🔍 *Confidence-based feedback loop:*
  - A softmax threshold was applied during training.
  - Predictions with low confidence were flagged and automatically looped back into training, improving accuracy on borderline cases.

- 🤖 *Semi-Supervised Learning:*
  - Unlabeled samples were introduced gradually.
  - Pseudo-labels were generated and refined using a *self-training mechanism*.

- 🔄 *Data Augmentation:*
  - Techniques such as rotation, flipping, zooming, and color variation were applied to increase training data diversity and reduce overfitting.

> 🚧 *Note:* Due to plans for scientific publication, implementation specifics are intentionally withheld at this stage.


## ⚙ Tools & Libraries

- *Python*
- *TensorFlow, **Keras*
- *Pandas, **NumPy, **Scikit-learn*
- *OpenCV*
- *Matplotlib, **Seaborn*


## 🚀 Development Platform

Model development and training were performed on *Google Colab* with GPU acceleration for efficient experimentation.


## 📊 Results Summary

- Best-performing model: *VGG (fine-tuned)*
- Semi-supervised learning led to *notable performance improvements*
- Achieved high classification accuracy even on *non-preprocessed, real-world images*


## 📁 Suggested Repository Structure

```plaintext
project-root/
│
├── README.md
├── dataset/
├── notebooks/
├── models/
├── utils/
└── results/




📬 Contact

mahdis.kh1134@gmail.com"
