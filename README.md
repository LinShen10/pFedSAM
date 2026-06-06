# pFedSAM: Dual-Personalized Federated Learning for Multi-Site ADHD Classification

## Overview

This repository provides the official implementation of **pFedSAM**, a novel dual-personalized federated learning framework for multi-site ADHD classification using multimodal neuroimaging data.

------

## Project Structure

pFedSAM/

├── data/                     # Dataset storage and preprocessing

├── federated/                # Federated learning workflow

│   ├── client.py             # Client-side local training and updates

│   └── server.py             # Server-side aggregation and coordination

├── models/                   # Neural network architectures

│   ├── base_models.py        # Base model definitions

│   ├── client_model.py       # Personalized client models

│   └── nas_modules.py        # Neural architecture search related modules

├── utils/                    # Utility functions

│   ├── helpers.py            # Common helper functions

│   └── metrics.py            # Evaluation metrics

├── config.py                 # Experimental configurations

└── main.py                   # Entry point for training and evaluation


## Dataset

Experiments are conducted on:

- ADHD-200 Dataset
- ABIDE-I Dataset

### Modalities

- Resting-state fMRI
- Structural MRI (sMRI)

### Brain Atlas

- CC200 atlas (200 ROIs)
