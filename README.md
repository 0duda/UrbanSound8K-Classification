# UrbanSound8K Classification using Deep Learning

A comprehensive study comparing **CNNs** and **MLPs** for environmental sound classification on the UrbanSound8K dataset, with adversarial robustness analysis using DeepFool attacks.

## Project Overview

This project implements and evaluates multiple deep learning architectures for classifying urban sounds into 10 categories:
- Air Conditioner
- Car Horn
- Children Playing
- Dog Barking
- Drilling
- Engine Idling
- Gunshot
- Jackhammer
- Siren
- Street Music

## Key Features

**Multiple Feature Representations**: Mel Spectrograms, MFCCs, and combined Mel+MFCC  
**Architecture Comparison**: CNN vs MLP vs Ensemble  
**Advanced Preprocessing**: Data augmentation with SpecAugment, time-stretch, pitch-shift  
**10-Fold Cross-Validation**: Rigorous evaluation protocol  
**Adversarial Robustness**: DeepFool attack analysis on trained models  
**Production-Ready Code**: Caching, efficient data pipelines, model checkpointing  

**Best Model**: CNN trained on Mel Spectrograms with 10-fold cross-validation

## Project Structure

```
UrbanSound8K-Classification/
├── CNN.ipynb                   # CNN implementation (Mel, MFCC, Both)
├── MLP.ipynb                   # MLP baseline and hyperparameter tuning
├── DEEPFOOL_CNN.ipynb          # Adversarial robustness analysis for CNN
├── DEEPFOOL_MLP.ipynb          # Adversarial robustness analysis for MLP
├── PROJECT.ipynb               # Initial data analysis
├── requirements.txt            # Python dependencies
├── presentations_slides.pdf    # Slides used for presentation 
├── AC2_Project_20252026.pdf    # Assignment
├── README.md                   # This file
└── SETUP.md                    # Guide for running the project
```

## Dependencies

- Python 3.8+
- TensorFlow 2.10+
- NumPy, Pandas, Scikit-learn
- Librosa (audio processing)
- Matplotlib, Seaborn (visualization)

See `requirements.txt` for exact versions.

## Authors
- Carolina Proença
- Eduarda Neves
- Maria Morais

**Note**: The UrbanSound8K dataset is not included in this repository due to size constraints (~6GB). Download it separately from the [official source](https://urbansounddataset.org/).
