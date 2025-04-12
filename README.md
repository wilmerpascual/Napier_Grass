# Napier_Grass
Project Overview
Napier grass (Pennisetum purpureum), a critical livestock forage in tropical regions, faces significant yield losses (20-50%) due to pests and diseases. This project implements a dual Convolutional Neural Network (CNN) system using InceptionV3 to:

Binary Classification: Distinguish Napier grass from non-Napier entities (e.g., weeds, similar crops) with 83.90% accuracy.
Multiclass Classification: Detect 12 pest/disease classes plus a healthy class with 94.00% accuracy.
Integrated with smartphone imaging, this system empowers smallholder farmers to monitor crops efficiently, potentially reducing yield losses by 20-30%. The project aligns with Sustainable Development Goals (SDGs) 2 (Zero Hunger), 12 (Responsible Consumption), and 15 (Life on Land).

This repository contains:

Training scripts for InceptionV3, VGG16, and DenseNet models implemented in TensorFlow/Keras.
Configurations for image preprocessing and data augmentation.
Sample code for model evaluation and prediction.
The full dataset (6,400 binary and 4,160 multiclass images) is available upon request, subject to approval from Marinduque State University, as detailed in the paper.

Purpose of this Repository
This README guides users in:

Setting up the environment to replicate the study.
Running the CNN models for training, evaluation, or inference.
Understanding the preprocessing pipeline for Napier grass images.
The code is intended for researchers in precision agriculture, computer vision, or AI for sustainability, as well as developers building farmer-friendly tools.

Key Features
Binary Classification: Identifies Napier grass vs. non-Napier entities (e.g., Mombasa grass, corn).
Multiclass Classification: Detects 12 pest/disease classes (e.g., fungal blast, planthoppers) and healthy Napier grass.
Smartphone Compatibility: Optimized for ≥12MP images captured under natural daylight.
Transfer Learning: Leverages pre-trained InceptionV3 weights for robust performance on limited data.
Reproducible Workflow: Includes preprocessing (resizing, normalization, augmentation) and evaluation metrics (Accuracy, Precision, Recall, F1 Score).




Getting Started
Prerequisites
Hardware: GPU recommended (e.g., NVIDIA CUDA-compatible for TensorFlow).
Software:
Python 3.8+
TensorFlow 2.10+ (GPU support optional)
Keras
NumPy, OpenCV, Matplotlib
Dataset: Request access to the 6,400 binary and 4,160 multiclass images via [contact details below].

Dataset Access
The dataset includes:

Binary: 6,400 images (3,200 Napier, 3,200 non-Napier).
Multiclass: 4,160 images (13 classes, 320 each). To request access, contact [pascual.wilmer@marsu.edu.ph] with your research purpose. Sample images may be included in /data/sample/ for testing.


Limitations
Dataset sourced primarily from Marinduque, Philippines, which may limit generalizability.
Binary model shows slight overfitting (98.02% training vs. 83.90% validation accuracy).
Smartphone inference requires ≥12MP cameras and stable lighting.
Future Work
Expand dataset with multi-region images.
Test advanced architectures (e.g., EfficientNet).
Develop a mobile app for real-time monitoring.
Optimize for edge devices with lower computational resources.
Citation
If you use this code or dataset, please cite:
Pascual, W. M., & Malinao, R. M. L. (2025). Leaf Intelligence: Advancing Napier Grass Monitoring with Binary and Multiclass CNN Classification. [TBA].


Contact
For questions or dataset requests, reach out to:

Wilmer M. Pascual: [pascual.wilmer@marsu.edu.ph]


Acknowledgments
We thank Marinduque State University, local farmers, and agronomists for their support in data collection and validation.
