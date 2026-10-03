# 🌿 Malabar Spinach Leaf Disease Segmentation

This repository contains a comparative deep learning study for **semantic segmentation of diseased regions in Malabar spinach (*Basella alba*) leaves**.

The objective is to accurately segment disease-affected regions from leaf images and compare the performance of different semantic segmentation architectures for automated agricultural disease analysis.

## 🧠 Segmentation Models

Five deep learning architectures are evaluated:

* **U-Net**
* **U-Net++**
* **Attention U-Net**
* **SegNet**
* **DeepLabV3**

## 🦠 Diseases

The study considers three Malabar spinach leaf diseases:

* **Bacterial Spots**
* **Downy Mildew**
* **Anthracnose**

## 📌 Project Objectives

This project aims to:

* Segment disease-affected regions from Malabar spinach leaf images
* Compare the performance of multiple segmentation architectures
* Evaluate model performance for individual diseases
* Perform overall evaluation across the complete test set
* Provide reproducible training and testing notebooks
* Release trained model weights for further research and experimentation

## 📂 Repository Structure

```text
Segmentation_of_Malabar_spinach/
│
├── UNet/
│   ├── unet_segmentation_training.ipynb
│   ├── unet-testing_bacterial_spots.ipynb
│   ├── unet-testing_anthracnose.ipynb
│   ├── unet-testing_downy_mildew.ipynb
│   └── unet-testing_overall.ipynb
│
├── UNet++/
│   ├── u_net++_segmentation_training.ipynb
│   ├── u-net++-testing_bacterial_spots.ipynb
│   ├── u-net++-testing_anthracnose.ipynb
│   ├── u-net++-testing_downy_mildew.ipynb
│   └── u-net++-testing_overall.ipynb
│
├── Attention_UNet/
│   ├── ...
│
├── SegNet/
│   ├── ...
│
├── DeepLabV3/
│   ├── ...
│
└── README.md
```

Each model directory contains:

* ✅ **1 training notebook**
* ✅ **3 disease-specific testing notebooks**
* ✅ **1 overall testing notebook**

## 🗂 Dataset

The dataset consists of Malabar spinach leaf images containing three disease categories:

* Bacterial Spots
* Downy Mildew
* Anthracnose

### Original Dataset

The leaf image dataset was obtained from the dataset published with the following scientific data article:

[ScienceDirect – Malabar spinach dataset](https://www.sciencedirect.com/science/article/pii/S2352340925000253)

### Kaggle Resources

**Leaf Image Dataset:**
[Malabar Dataset – Kaggle](https://www.kaggle.com/datasets/ragibmehedi/malabar-dataset)

**LabelMe JSON Annotations:**
[Malabar Dataset – Annotated JSON Files](https://www.kaggle.com/datasets/ragibmehedi/malabar-dataset-annotated-json-files)

**Trained Model Weights:**
[Malabar Spinach Keras Files – Kaggle](https://www.kaggle.com/datasets/ragibmehedi/malabar-spinach-keras-files)

## 🏷️ Annotation

Pixel-wise annotations were created for the disease-affected regions of the leaves.

The following disease categories were annotated:

* Bacterial Spots
* Downy Mildew
* Anthracnose

**LabelMe** was used to create polygon-based annotations. The corresponding binary segmentation masks were generated from the LabelMe JSON annotation files.

## 💾 Model Weights

The best-performing model weights obtained during training are provided as `.keras` files.

These weights can be used to reproduce the testing experiments or perform inference on new images.

## 📊 Evaluation

The models are evaluated using pixel-level semantic segmentation metrics, including:

* **Intersection over Union (IoU)**
* **Dice coefficient**

Evaluation is performed both:

1. **Disease-wise**, for Bacterial Spots, Downy Mildew, and Anthracnose
2. **Overall**, across the complete test dataset

## 🔬 Reproducibility

The repository provides the training and testing notebooks used in the experiments.

The notebooks include the necessary steps for:

* Dataset preparation
* Loading and preprocessing images
* Loading segmentation masks
* Model training
* Model evaluation
* Disease-specific testing
* Overall testing
* Saving and loading trained model weights


---


