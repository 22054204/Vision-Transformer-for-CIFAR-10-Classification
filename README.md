# Vision Transformer for CIFAR-10 Classification

**Assignment 4 – Vision Transformer Implementation**  
**Name:** Ranjan Sharma  
**Roll Number:** 22054204  
**Section:** CSE 24  
**Model Name:** CIFARViT_404

---

## Overview

This project implements a Vision Transformer (ViT) from scratch for image classification on the CIFAR-10 dataset. The model features 6 transformer encoder layers with multi-head self-attention mechanisms.

## Model Architecture

- **Layers:** 6 Transformer Encoder Blocks
- **Hidden Dimension:** Roll-derived (adjusted for head divisibility)
- **Attention Heads:** Roll-dependent (3-7 heads)
- **Patch Size:** Roll-dependent (10-14 pixels)
- **Activation:** ReLU
- **Normalization:** LayerNorm

## Configuration

```python
ROLL_ID = 22054204
Learning Rate: 5e-4
Batch Size: 128
Optimizer: Adam
LR Scheduler: StepLR (step_size=5, gamma=0.7)
```

## Dataset

- **CIFAR-10:** 10 classes (airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck)
- **Training:** 45,000 images
- **Validation:** 5,000 images
- **Test:** 10,000 images
- **Image Size:** 32×32 RGB

## Installation

### Google Colab
```python
!pip install torch torchvision scikit-learn matplotlib -q
```

### Local
```bash
pip install torch torchvision scikit-learn matplotlib numpy
```

## Usage

1. Upload `Assignment4_ViT_RanjanSharma_22054204.ipynb` to Google Colab
2. Run all cells
3. Results saved in `/content/vit_404/`
4. Zip file automatically downloaded

## Output Files

- **model_404.pth** - Trained model weights
- **curve_404.png** - Training and validation accuracy curves
- **cm_404.png** - Confusion matrix
- **att_404.png** - Attention map visualization
- **vit_404.zip** - All outputs compressed

## Features

- Patch-based image processing
- Multi-head self-attention mechanism
- Residual connections
- Learnable position embeddings
- CLS token for classification
- Attention visualization
- Reproducible results with fixed seeds

---

**Note:** Designed for Google Colab but adaptable for local execution.
