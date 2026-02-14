🌿 Malabar Spinach Leaf Disease Segmentation

This repository presents a comparative deep learning study for semantic segmentation of Malabar Spinach leaf diseases. The goal is to accurately segment diseased regions from leaf images to assist in automated agricultural disease analysis.

The project evaluates five state-of-the-art segmentation architectures:

UNet

UNet++

Attention UNet

SegNet

DeepLabV3

The diseases considered in this study are:

Bacterial Spots

Downy Mildew

Anthracnose

📌 Project Objective

Manual disease detection in crops is labor-intensive and error-prone. This project aims to:

Segment infected regions from leaf images

Compare performance of multiple segmentation models

Analyze disease-wise performance

Provide reproducible experimental pipelines

📂 Repository Structure
Segmentation_of_Malabar_spinach
│
├── UNet/
│   ├── unet_segmentation_training.ipynb
│   ├── unet-testing_bacterial_spots.ipynb
│   ├── unet-testing_anthracnose.ipynb
│   ├── unet-testing_downy_mildew.ipynb
│   ├── unet-testing_overall.ipynb
│
├── UNet++/
│   ├── u_net++_segmentation_training.ipynb
│   ├── u-net++-testing_bacterial_spots.ipynb
│   ├── u-net++-testing_anthracnose.ipynb
│   ├── u-net++-testing_downy_mildew.ipynb
│   ├── u-net-testing_overall.ipynb
│
├── Attention_UNet/
├── SegNet/
├── DeepLabV3/
│
└── README.md


Each model folder contains:

✅ 1 Training Notebook

✅ 3 Disease-Specific Testing Notebooks

✅ 1 Overall Testing Notebook


🗂 Dataset Description

The main dataset consists of leaf images of Malabar spinach

Original link : https://www.sciencedirect.com/science/article/pii/S2352340925000253 

kaggle link of my dataset : https://www.kaggle.com/datasets/ragibmehedi/malabar-dataset

kaggle link of .json files : https://www.kaggle.com/datasets/ragibmehedi/malabar-dataset-annotated-json-files

The best weights were stored in .keras files. Link: https://www.kaggle.com/datasets/ragibmehedi/malabar-spinach-keras-files

Pixel-wise annotation for:

Bacterial Spots

Downy Mildew

Anthracnose

LabelMe was used for annotation and binary masks were generated from JSON files.
