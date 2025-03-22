# Plaque Classifier

A repository for building and training machine learning models to classify amyloid plaque images, aiding Alzheimer's research and diagnostics. This repository was created as a part of a manuscript that is currently under review.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Usage](#usage)
- [Pre-requisites](#pre-requisites)

## Introduction
Amyloid plaques are hallmark indicators of Alzheimer's disease. This project leverages advanced image processing and machine learning techniques to classify amyloid plaque images accurately, potentially contributing to early diagnosis and research efforts.

## Features
- Preprocessing tools for image datasets
- Convolutional Neural Network (CNN) model for plaque classification
- K-Fold cross-validation for robust training
- Data augmentation for improved generalization
- Model checkpointing and training logs
- Prediction scripts

## Usage
### Training the Model
To train the model, use the plaque_classifier_training.ipynb, which implements K-Fold cross-validation to train the CNN model. The training pipeline consists of:
1. **Loading Images**: Converts images to grayscale and resizes them.
2. **Preprocessing**: Normalizes pixel values and converts labels to categorical format.
3. **Model Training**: Uses a CNN architecture with five convolutional layers and dropout regularization.
4. **Data Augmentation**: Applies transformations to enhance training robustness.
5. **Evaluation**: Implements Stratified K-Fold cross-validation and logs accuracy and loss metrics. 

### Making Predictions
A separate script (plaque_classifier_prediction.ipynb) for making predictions will load the trained model and classify new plaque images.

## Pre-requisites
This software was developed in Python 3.7.3. The project was developed and is generally deployed using NVIDIA GeForce RTX 2080 Ti. TensorFlow was accelerated using this GPU via CUDA (10.1.243) and CUDANN (7.6.5).

General guidelines for prerequisites:
- Install Anaconda and make sure GPU drivers are up-to-date.
- In a PowerShell/terminal supported by Anaconda, create a new virtual environment to run this project:
  ```sh
  conda create -n "plaque_env" python=version_appropriate_for_tensorflow_and_gpu ipython
  ```
- Activate the environment:
  ```sh
  conda activate plaque_env
  ```
- Install packages from the `requirements.txt` file:
  ```sh
  pip install -r requirements_scandx_concise.txt
  ```

The demo should be expected to run for less than one minute and installation should not take more than one hour.
