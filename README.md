# 🧬 Cell Nuclei Segmentation using U-Net (DSB 2018)

A deep learning project for nuclei (cell instance) segmentation using a
custom U-Net Encoder-Decoder architecture implemented with
TensorFlow/Keras.

The model performs pixel-level binary segmentation to detect and
separate cell nuclei in microscopy images from the Kaggle Data Science
Bowl 2018 dataset.

<img width="183" height="214" alt="cell" src="https://github.com/user-attachments/assets/a6fc40ca-4620-4803-9d5d-8a003e7a8845" /> <img width="183" height="214" alt="cell - Copy" src="https://github.com/user-attachments/assets/c0c539d2-a9e0-4966-91bd-1abac29854d3" /> <img width="183" height="214" alt="cell - Copy (2)" src="https://github.com/user-attachments/assets/5ec83b38-c6d8-4445-92c8-adbc98a4bfac" />


This project is widely applicable in:

-   Medical Image Analysis
-   Cancer Research
-   Pathology Assistance Systems
-   Biomedical Computer Vision
-   Cell Detection & Quantification

------------------------------------------------------------------------

# 📌 Project Overview

Cell nuclei segmentation is a fundamental task in biomedical image
analysis where each pixel is classified as either nucleus or background.

In this project, a U-Net based deep learning model is trained to
generate high-quality binary segmentation masks for microscopy images
with varying shapes, densities, and imaging conditions.

## Model Workflow

Input Microscopy Image \| v U-Net Encoder-Decoder Network \| v
Pixel-wise Binary Prediction \| v Nuclei Segmentation Mask

------------------------------------------------------------------------

# 🏗️ Model Architecture

The model is based on a custom U-Net-style encoder-decoder CNN with skip
connections for preserving spatial details.

## Encoder

Conv Block (32) -\> Conv Block (64) -\> Conv Block (128) -\> Conv Block
(256)

Each block: - Conv2D (3x3) - ReLU - MaxPooling

## Decoder

UpConv + Skip Connections -\> Refinement Conv layers

## Output Layer

Conv2D(1x1, sigmoid)

------------------------------------------------------------------------

# 📂 Project Structure

```
people-clothing-segmentation/
│
├── Data/
├── stage1_train/
│   ├── <Image_ID>/
│   │   ├── images/
│   │   └── masks/
│   ├── ...
│   ├── stage1_test/
│   └── stage2_test_final/
│
├── Notebooks/
│   └── cell-instance-segmentation.ipynb
│
├── Requirements.txt
└── README.md
```

------------------------------------------------------------------------

# 🧪 Dataset

Kaggle Data Science Bowl 2018: - Variable image sizes - Different
microscopy conditions - Dense/sparse nuclei regions - Pixel-level
annotations

------------------------------------------------------------------------

# 🛠️ Technologies

Python, TensorFlow, Keras, OpenCV, NumPy, Matplotlib, Scikit-learn

------------------------------------------------------------------------

# 📊 Metrics

-   Binary Cross-Entropy Loss

------------------------------------------------------------------------

------------------------------------------------------------------------

# 👨‍💻 Author :Ramin Allahverdizadeh

U-Net biomedical segmentation project using TensorFlow/Keras
