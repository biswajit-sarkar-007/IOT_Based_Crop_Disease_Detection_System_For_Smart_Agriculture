---
license: cc-by-4.0
language:
- en
task_categories:
- image-classification
task_ids:
- multi-class-classification
pretty_name: Crop Disease Image Dataset (5 Crops, 19 Classes)
size_categories:
- 10K<n<100K
---

#  Crop Disease Image Dataset (5 Crops, 19 Classes)

## Dataset Description

This dataset is a **custom crop disease image dataset** developed for research in **Artificial Intelligence, Deep Learning, Computer Vision, and Smart Agriculture**.

The dataset was created by combining and organizing images collected from multiple publicly available datasets. It contains leaf images from **five major crops** with both healthy and diseased classes.

The dataset is intended for developing image classification models such as **MobileNetV3, ResNet, EfficientNet, Vision Transformers (ViT),** and other deep learning architectures.

---

# Dataset Summary

| Property | Value                            |
|----------|----------------------------------|
| Total Crops | 5                                |
| Total Classes | 19                               |
| Total Images | 22,169                           |
| Image Format | JPG / JPEG                       |
| Dataset Size | ~1.36 GB                         |
| Task | Multi-class Image Classification |

---

# Crops Included

- 🌽 Corn (Maize)
- 🥔 Potato
- 🌾 Rice
- 🍅 Tomato
- 🌾 Wheat

---

# Class Distribution

##  Corn (Maize)

| Class | Images |
|--------|-------:|
| Cercospora Leaf Spot (Gray Leaf Spot) | 513 |
| Common Rust | 1,192 |
| Healthy | 1,662 |
| Northern Leaf Blight | 985 |
| Leaf Spot | 1,261 |
| Maize Streak Virus | 1,004 |

**Total Images:** **6,617**

---

##  Potato

| Class | Images |
|--------|-------:|
| Early Blight |  1,000 |
| Healthy |    968 |
| Late Blight |  1,000 |

**Total Images:** **2,968**

---

##  Rice

| Class | Images |
|--------|-------:|
| Brown Spot | 1,210 |
| Healthy | 1,470 |
| Leaf Blast | 957 |

**Total Images:** **3,637**

---

##  Tomato

| Class | Images |
|--------|-------:|
| Bacterial Spot | 2,127 |
| Early Blight | 1,000 |
| Healthy | 1,591 |
| Late Blight | 1,909 |

**Total Images:** **6,627**

---

##  Wheat

| Class | Images |
|--------|-------:|
| Brown Rust | 860 |
| Healthy | 1,080 |
| Yellow Rust | 880 |

**Total Images:** **2,820**

---

# Folder Structure

```
Crop_Disease_Image_Dataset/
│
├── Corn_(Maize)___Cercospora_Leaf_Spot_(Gray_Leaf_Spot)/
├── Corn_(Maize)___Common_Rust/
├── Corn_(Maize)___Healthy/
├── Corn_(Maize)___Northern_Leaf_Blight/
├── Corn_(Maize)___Leaf_Spot/
├── Corn_(Maize)___Maize_Streak_Virus/
│
├── Potato___Early_Blight/
├── Potato___Healthy/
├── Potato___Late_Blight/
│
├── Rice___Brown_Spot/
├── Rice___Healthy/
├── Rice___Leaf_Blast/
│
├── Tomato___Bacterial_Spot/
├── Tomato___Early_Blight/
├── Tomato___Healthy/
├── Tomato___Late_Blight/
│
├── Wheat___Brown_Rust/
├── Wheat___Healthy/
└── Wheat___Yellow_Rust/
```

---

# Recommended Data Split

For deep learning training, use a **stratified** dataset split to preserve the class distribution.

- **Training:** 70%
- **Validation:** 15%
- **Testing:** 15%

---

# Image Preprocessing

The original images are stored in their native resolutions.

During training, images can be preprocessed using **PyTorch Torchvision** transforms.

Typical preprocessing includes:

- Resize
- Center Crop
- Image Normalization
- Random Horizontal Flip
- Random Rotation
- Color Jitter (Optional)

The original dataset should remain unchanged.

---

# Applications

This dataset can be used for:

- Crop Disease Classification
- Healthy vs Diseased Classification
- Transfer Learning
- CNN Training
- MobileNetV3
- EfficientNet
- ResNet
- Vision Transformers (ViT)
- Agricultural AI Research
- Smart Farming Applications

---

# Source Datasets

This custom dataset was created by combining images from the following publicly available datasets.

## 1. PlantVillage Dataset

Repository:

- https://github.com/spMohanty/PlantVillage-Dataset


## 2. 15 Crop and 45 Disease and Healthy Dataset

Mendeley Data:

- https://data.mendeley.com/datasets/8fr7grr73p/1

---
# Source Datasets

- https://huggingface.co/datasets/ipartzix/Crop_Disease_Image_Dataset

---

# Citation

If you use this dataset in your research, academic work, or project, please cite:

```bibtex
@dataset{paul2026crop_disease_image_dataset,
  author       = {Partha Paul},
  title        = {Crop Disease Image Dataset},
  year         = {2026},
  publisher    = {Hugging Face},
  url          = {https://huggingface.co/datasets/ipartzix/Crop_Disease_Image_Dataset}
}
```

## 1. PlantVillage Dataset

**Research Paper**

Mohanty, S. P., Hughes, D. P., & Salathé, M. (2016). *Using deep learning for image-based plant disease detection*. Frontiers in Plant Science, 7, 1419.

DOI: https://doi.org/10.3389/fpls.2016.01419

**GitHub Repository**

https://github.com/spMohanty/PlantVillage-Dataset

---

## 2. 15 Crop and 45 Disease and Healthy Dataset

**Citation**

Jain, A. (2026). *15 Crop and 45 Disease and Healthy dataset* (Version 1). Mendeley Data.

DOI: https://doi.org/10.17632/8fr7grr73p.1


---

# License

This dataset is intended for **educational, academic, and research purposes**.

The images belong to their respective original dataset authors. This repository provides a cleaned and reorganized version for research and machine learning applications.

---

# Acknowledgements

We gratefully acknowledge the creators of:

- PlantVillage Dataset
- Mendeley Data (15 Crop and 45 Disease and Healthy Dataset)

for making their datasets publicly available for research.