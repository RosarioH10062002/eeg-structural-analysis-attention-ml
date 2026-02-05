# Structural Analysis of High-Dimensional EEG Signals using Machine Learning

This repository contains the code developed during a research internship (February–May 2025) under the supervision of **Dr. Axel Hutt**, focused on the analysis of high-dimensional EEG data using machine learning and statistical techniques.

The project explores how spectral features extracted from multichannel EEG recordings can be leveraged to characterize attentional states, identify redundancy across electrodes, and assess separability between attentive and inattentive groups.

---

## Project Overview

Electroencephalography (EEG) produces high-dimensional time-series data that require careful feature extraction and dimensionality reduction to reveal meaningful structure.  
In this project, full 64-channel EEG recordings were processed to extract frequency-domain features across canonical bands, followed by both supervised and unsupervised learning approaches.

The primary objectives were to:

- Characterize spectral signatures of attentional vs. inattentive states  
- Reduce dimensionality while preserving discriminative structure  
- Explore inter-channel relationships and synchrony patterns  
- Evaluate classification performance using interpretable machine learning models  

---

## Data Description

- **Modality:** EEG  
- **Channels:** 64 electrodes  
- **Features:**  
  - Delta power  
  - Alpha power  
  - Theta/Beta Ratio (TBR)  
- **Spatial focus:**  
  - Frontal site: Fpz  
  - Posterior site: Pz  
---

## Methods

### Feature Extraction
- Frequency-band power computed for all electrodes
- Targeted analysis on frontal and posterior regions
- Band-specific aggregation for delta, alpha, and TBR features

### Dimensionality Reduction
Used to identify redundancy and visualize group separability:
- Principal Component Analysis (PCA)
- Uniform Manifold Approximation and Projection (UMAP)
- t-distributed Stochastic Neighbor Embedding (t-SNE)

### Machine Learning
- **Supervised learning**
  - Support Vector Machines (SVM)
  - Extra Trees Classifier
  - Cross-validation for performance estimation
- **Unsupervised learning**
  - K-Means clustering
  - Hierarchical clustering

### Statistical Analysis
- Correlation analyses to assess inter-channel synchrony
- Regression analyses to explore accuracy and feature trends
