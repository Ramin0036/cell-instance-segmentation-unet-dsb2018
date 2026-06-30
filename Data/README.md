# 📂 Dataset

This project uses the **2018 Data Science Bowl** dataset from Kaggle for training and evaluating the nuclei segmentation model.

> **Dataset Link:**  
> https://www.kaggle.com/competitions/data-science-bowl-2018/data

---

# 📌 Why isn't the dataset included?

The original dataset is **too large** to be stored directly in this GitHub repository.

To keep the repository lightweight and easy to clone, the dataset has **not** been uploaded. Instead, please download it directly from the official Kaggle competition page using the link above.

---

# 🧬 About the Dataset

The **2018 Data Science Bowl** dataset is one of the most popular benchmark datasets for **cell nuclei segmentation** in biomedical image analysis.

It contains microscopy images collected from multiple laboratories under different experimental conditions, including:

- Fluorescence microscopy
- Brightfield microscopy
- Histology images
- Various cell types
- Multiple imaging resolutions

The diversity of imaging modalities and biological samples makes this dataset particularly challenging and suitable for developing robust deep learning segmentation models. :contentReference[oaicite:0]{index=0}

---

# 📁 Dataset Structure

After downloading and extracting the dataset, organize it as follows:

```text
dataset/
│
├── stage1_train/
│   ├── <Image_ID>/
│   │   ├── images/
│   │   └── masks/
│   ├── ...
│
├── stage1_test/
│
└── stage2_test_final/
```

Each training sample contains:

- **images/** → Original microscopy image
- **masks/** → Individual binary mask for each nucleus

Each mask corresponds to **exactly one cell nucleus**, making the dataset suitable for instance segmentation tasks. :contentReference[oaicite:1]{index=1}

---

# 📊 Dataset Highlights

- 🧫 800+ microscopy images
- 🔬 More than **37,000** manually annotated cell nuclei
- 🧬 Multiple organisms (Human, Mouse, Fly)
- 📷 Various imaging modalities
- 🎯 Benchmark dataset for biomedical image segmentation

:contentReference[oaicite:2]{index=2}

---

# 🚀 Download

Download the dataset from the official Kaggle competition page:

https://www.kaggle.com/competitions/data-science-bowl-2018/data

After downloading, extract the files into the `dataset/` directory before running the training scripts.

---
