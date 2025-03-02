# Lung Cancer Severity Classification

This repository contains code and documentation for a deep learning project focused on lung cancer severity classification in CT scans. The project addresses both binary (benign/malignant) and 5-class malignancy scoring tasks.

## Datasets

The dataset consists of 512x512px grayscale CT scan slices from 2363 patients. For each CT scan, the slice with the largest nodule area was selected. In addition to each slice, a zoomed version of the nodule was also provided. The two types of images are in separate `.nrrd` files, and malignancy classes are in `dataset_lung.xlsx`.

![dataset](https://github.com/user-attachments/assets/d0b36e35-a4b1-4296-8c04-fcd98d93f6a5)

## Models

We explored a variety of deep learning models, including:

* ResNet50
* ConvNeXt
* Mushu (custom CNN)
* MedusaNet (custom CNN with inception blocks)
* Visual Transformers (ViT)

## Key Findings

* Deep Neural Networks (DNNs), specifically Deep Convolutional Neural Networks (DCNNs), were effectively employed for image classification.
* Data imbalance was a significant challenge, addressed through techniques like random rotations and loss weighting.
* Radiomics features proved beneficial for full-slice classification tasks.
* Explainable AI (XAI) methods, including Grad-CAM, were used to interpret model predictions.

## Contributors
* [Michele Bersani]()
* [Paolo Chiappini](https://github.com/paolo-chiappini) 
* [Andrea Fraschini](https://github.com/Andrea01Fraschini) 
* [Camilo José Sinning López](https://github.com/CamiloSinningUN)
