# Hybrid CNN–Transformer Framework for Structure-Preserving Enhancement of Coronary Angiography Images

This repository contains the implementation of the research paper:

**Hybrid CNN–Transformer Framework for Structure-Preserving Enhancement of Coronary Angiography Images**

## Authors
- Romaan Khan  
- Abdullah  
- Islam Uddin  
- Salman Khan  

## Overview
Coronary artery disease (CAD) is a leading cause of mortality worldwide. X-ray coronary angiography is widely used for diagnosing coronary artery conditions; however, angiographic images often suffer from **low contrast, noise, motion blur, and compression artifacts**.

This project proposes a **hybrid deep learning framework combining Convolutional Neural Networks (CNNs) and Transformer-based self-attention mechanisms** for enhancing coronary angiography images while preserving fine vascular structures and global anatomical continuity.

The proposed model integrates:

- **CNN modules** for local feature extraction and noise suppression
- **Transformer modules** for global contextual modeling
- **Feature fusion mechanisms** for structure-preserving reconstruction

## Key Features
- Hybrid **CNN–Transformer architecture**
- Structure-preserving angiography image enhancement
- Local–global feature fusion
- Improved reconstruction fidelity
- Quantitative and qualitative evaluation

## Dataset
The experiments were conducted using the **ARCADE Coronary Angiography Dataset**.

Dataset link:
https://drive.google.com/drive/folders/1FO1OHak0S9kFRt4kszr7S73dQ7Mcq5NB?usp=drive_link 
Dataset split used in the study:

| Dataset | Images |
|-------|-------|
| Training | 1000 |
| Validation | 300 |
| Testing | 300 |
| Total | 1600 |

## Model Architecture
The framework consists of three main modules:

1. **CNN Encoder**
   - Extracts hierarchical local features
   - Suppresses noise and restores vessel edges

2. **Transformer Module**
   - Captures long-range spatial dependencies
   - Maintains global vessel continuity

3. **Reconstruction Decoder**
   - Fuses local and global features
   - Generates enhanced angiography images

## Training Configuration

| Parameter | Value |
|----------|------|
| Optimizer | Adam |
| Learning Rate | 1e-4 |
| Batch Size | 4 |
| Loss Function | MSE |
| Input Image Size | 128 × 128 |
| Weight Decay | 1e-5 |
| Early Stopping | 10 epochs |

## Evaluation Metrics
Model performance is evaluated using:

- **PSNR (Peak Signal-to-Noise Ratio)**
- **SSIM (Structural Similarity Index Measure)**

### Results

| Model | PSNR | SSIM |
|------|------|------|
| CNN Baseline | 33.69 | 0.9594 |
| Transformer Only | 34.21 | 0.9612 |
| Proposed Hybrid CNN–Transformer | **36.10** | **0.9670** |

## Repository Structure

## Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/hybrid-cnn-transformer-angiography.git
pip install -r requirements.txt
python train.py
python evaluate.py
RK-IU/
├─ data/
│  ├─ train/
│  ├─ validation/
│  └─ test/
├─ models/
│  ├─ cnn_encoder.py
│  ├─ transformer_module.py
│  └─ hybrid_model.py

## Repository Structure
## Repository Structure

- **data/**
  - train/
  - validation/
  - test/

- **models/**
  - cnn_encoder.py
  - transformer_module.py
  - hybrid_model.py

- **training/**
  - train.py
  - loss_functions.py

- **evaluation/**
  - metrics.py
  - evaluation.py

- **configs/**
  - config_0.json
  - config_1.json
  - config_2.json

- **notebooks/**
  - hybrid_model_demo.ipynb

- **results/**
  - figures/
  - outputs/

- **README.md**

```
