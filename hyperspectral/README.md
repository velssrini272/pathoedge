# 1D-CNN Hyperspectral Classification

## Overview
This project implements a One-Dimensional Convolutional Neural Network (1D-CNN) for classification of hyperspectral data.

The model learns spectral patterns from wavelength-wise measurements and predicts the corresponding class.

## Workflow

Hyperspectral Data
        ↓
Data Preprocessing
        ↓
Spectral Feature Extraction
        ↓
1D-CNN Model
        ↓
Training & Validation
        ↓
Class Prediction
        ↓
Accuracy / Confusion Matrix

## Model
The 1D-CNN processes spectral information as a one-dimensional sequence.

Main stages:
- Conv1D layers
- Activation
- Pooling
- Flattening
- Fully Connected layer
- Softmax classification

## Training
The model is trained using labelled hyperspectral samples.

Training includes:
- Dataset preparation
- Train/validation split
- Model training
- Validation
- Performance evaluation

## Output
The trained model produces:
- Predicted class labels
- Classification accuracy
- Confusion matrix
- Per-class performance

## Application to PathoEdge
For PathoEdge, the same 1D-CNN concept can be applied to spectral responses captured from food surfaces under sequential UV/NIR illumination.

The model can classify the measured spectral patterns into:

- PASS
- UNCERTAIN
- REJECT

The trained model can then be converted to a lightweight TensorFlow Lite model for edge deployment with a Coral TPU.
