# PyTorch ResNet Implementation

This repository contains a PyTorch implementation of the ResNet (Residual Network) architecture, specifically including ResNet50, ResNet101, and ResNet152 variants.

## Overview

ResNet is a powerful convolutional neural network architecture that introduced skip connections to solve the vanishing gradient problem in deep networks. This implementation includes:

- A basic `block` class that defines the structure of residual blocks
- A `ResNet` class that constructs the full network
- Functions to create ResNet50, ResNet101, and ResNet152 models
- A test function to verify the implementation

## Requirements

- PyTorch
- torchvision (for dataset loading and preprocessing, if needed)

## Usage

To use this implementation, simply import the desired ResNet variant:

```python
from resnet import ResNet50, ResNet101, ResNet152

# Create a ResNet50 model
model = ResNet50(img_channels=3, num_classes=1000)

# Create a ResNet101 model
model = ResNet101(img_channels=3, num_classes=1000)

# Create a ResNet152 model
model = ResNet152(img_channels=3, num_classes=1000)
