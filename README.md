# Plaque Classifier

A repository for building and training machine learning models to classify amyloid plaque images, aiding Alzheimer's research and diagnostics.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)

## Introduction
Amyloid plaques are hallmark indicators of Alzheimer's disease. This project leverages advanced image processing and machine learning techniques to classify amyloid plaque images accurately, potentially contributing to early diagnosis and research efforts.

## Features
- Preprocessing tools for image datasets
- Pre-trained deep learning models
- Prediction scripts

## Pre-requisites
This software was developed in Python 3.7.3. The project was developed and is generally deployed using NVIDIA GeForce RTX 2080 Ti. Tensorflow was accelerated using this GPU via CUDA (10.1.243) and CUDANN (7.6.5).
General guidelines for prerequisites
- Install Anaconda and make sure GPU drivers are up-to-date
- In a powershell/terminal supported by Anaconda, create a new virtual environment to run this project. You can simply copy the code:
conda create -n "plaque_env" python=version_appropriate_for_tensorflow_and_gpu ipython
- Activate the environment
conda activate plaque_env
- Install packages from the file "requirements.txt" file:
pip install -r requirements_scandx_concise.txt
