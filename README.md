# pFedSAM: Dual-Personalized Federated Learning for Multi-Site ADHD Classification

## Overview

This repository provides the official implementation of **pFedSAM**, a novel dual-personalized federated learning framework for multi-site ADHD classification using multimodal neuroimaging data.

The proposed framework jointly addresses:

- **Cross-site data heterogeneity**
- **Multimodal discrepancy between fMRI and sMRI**
- **Personalization in federated medical imaging**

by integrating:

- **Modality-Guided Domain Adaptation**
- **Source-Anchored Alignment Mechanism**
- **Dual-Level Personalized Federated Learning**
- **Neural Architecture Search (NAS)**

The framework leverages the structural stability of sMRI to guide the alignment of more heterogeneous fMRI representations, enabling robust cross-site multimodal learning under privacy-preserving federated settings.

------

## Key Features

### 1. Modality-Guided Alignment

- Uses stable sMRI representations as structural anchors
- Guides fMRI feature alignment across modalities and sites
- Reduces both modality and domain discrepancies

### 2. Source-Anchored Mechanism

- Introduces EMA-based global prototypes
- Provides stable cross-round feature alignment
- Improves federated optimization stability

### 3. Dual Personalization

- Parameter-Level Personalization
  - Wasserstein-distance-based adaptive aggregation
- Architecture-Level Personalization
  - Client-specific NAS optimization using Gumbel-Softmax

### 4. Multi-Level Domain Adaptation

The framework performs alignment at:

- Sample level
- Distribution level
- Domain level
- Global level

------

## Framework Architecture

The proposed pFedSAM framework contains:

- Federated multimodal learning pipeline
- Modality-guided feature alignment
- Source-domain anchored consistency learning
- Personalized aggregation
- Differentiable NAS architecture search

------

## Dataset

Experiments are conducted on:

- ADHD-200 Dataset
- ABIDE-I Dataset

### Modalities

- Resting-state fMRI
- Structural MRI (sMRI)

### Brain Atlas

- CC200 atlas (200 ROIs)
