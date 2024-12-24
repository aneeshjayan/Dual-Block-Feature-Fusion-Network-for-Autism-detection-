# Autism Spectrum Disorder (ASD) Classification with Dual-Track Feature Fusion and Quantum Machine Learning

This repository contains the implementation of a novel hybrid framework for classifying Autism Spectrum Disorder (ASD) using Magnetic Resonance Imaging (MRI) data. The project integrates cutting-edge deep learning and quantum machine learning techniques to achieve high classification accuracy.

## Features

- **Dual-Track Feature Fusion**:
  - **Swin Transformer**: Captures global dependencies in MRI images through a hierarchical approach and shifted windows.
  - **Custom CNN**: Extracts local spatial features using a 2D convolutional neural network with progressive feature extraction.

- **Quantum Support Vector Machine (QSVM)**:
  - Quantum computing-based classification using quantum feature maps and kernel functions.

- **High Accuracy**:
  - Achieved 98.7% accuracy with the ABIDE-I dataset.
  - Validated with ABIDE-II dataset, achieving 96.82% accuracy.

## Architecture

1. **Dual-Track Feature Extraction**:
   - Global features extracted by Swin Transformer.
   - Local features extracted by Custom CNN.

2. **Feature Fusion**:
   - Features from both models are reduced using PCA and fused for classification.

3. **Classification**:
   - Multilayer Perceptron (MLP) for initial classification.
   - Quantum SVM for advanced classification leveraging quantum computing principles.

## Datasets

- **ABIDE-I**: Used for training and testing.
- **ABIDE-II**: Used for independent validation.
  - Data split: 80% training, 10% validation, 10% testing.
  - Includes 2D MRI slices derived from original NIfTI files.

## Performance Metrics

| Model             | Accuracy | Precision | Recall | F1-Score |
|--------------------|----------|-----------|--------|----------|
| Swin Transformer  | 90.17%   | 90.18%    | 90.85% | 90.27%   |
| Custom CNN        | 95.12%   | 95.50%    | 96.34% | 95.88%   |
| Hybrid Model (MLP)| 98.7%    | 98.12%    | 98.77% | 98.65%   |
| QSVM              | 96%      | 96.66%    | 96.12% | 96.88%   |
