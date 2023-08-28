# Neural-Decoding-fMRI-AlexNet-MLP
Neural Decoding of Image Classes using fMRI with AlexNet and MLP
# Neural Decoding of Image Classes using fMRI with AlexNet and MLP

**Authors:** Farnaz Garehdaghi, Medha Shekhar, Taraneh Attary, Reza Tondfekr, Mina Rezaie (project TA), Hazrat Ali (project mentor)

This project focuses on decoding neural responses using deep learning techniques to understand how the brain represents information. The goal is to predict image identities based on fMRI activations and compare these representations with features from pretrained AlexNet. The project bridges neuroscience and computer vision, potentially aiding image recognition and decoding human brain responses to visual stimuli.

## Dataset

The dataset used is the Kay fMRI dataset (Kay et al, 2008), containing fMRI responses to images. The dataset consists of 1750 training stimuli images and 120 testing stimuli images, categorized into 8 classes. Each stimuli has 8428 voxel responses from 8 brain regions.

## Goals

- Train a 4-layer MLP network to classify images from two classes: animals vs artifacts.
- Fine-tune a pretrained AlexNet on fMRI data and compare its features with features from an AlexNet trained on images.

## Procedure

1. Balanced dataset: Reduced classes to animals vs artifacts, with equalized images (589 each).
2. Data augmentation: Increased data by randomly selecting voxels for new inputs.
3. MLP network: Trained on fMRI responses from different brain areas (V1, V4, LOC), achieving ~70% accuracy for LOC.
4. AlexNet fine-tuning: Last layer fine-tuned on fMRI responses, features compared with AlexNet trained on images.
5. Evaluation: Accuracy, confusion matrix, ROC curves, pearson correlation coefficient used for evaluation.

## Reference Papers

1. Identifying natural images from human brain activity (K. N. Kay et al.)
2. Imagenet classification with deep convolutional neural networks (A. Krizhevsky et al.)

## Abstract

This project investigates decoding neural responses using an MLP network and comparing brain representations with features from a pretrained AlexNet. A 4-layer MLP achieved ~70% accuracy for semantic labels in the LOC brain area. AlexNet fine-tuning is used to predict fMRI responses, with feature representations compared. The project merges neuroscience and computer vision, revealing brain regions correlated with image features.



