# Spiking Zoo

Spiking Zoo is a Python library designed to wrap and standardize several Spiking Neural Network (SNN) models for inference. The goal is to provide a consistent interface for loading, preprocessing, running inference, and postprocessing across various SNN models.

## Table of Contents
- [Overview](#overview)
- [File Structure](#file-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)


## Overview

This library defines a base class (`BaseModel`) to enforce a standard interface for all SNN models, enabling easy model integration and management. It currently includes implementations for:
- **Spiking ResNet**
- **Spiking VGG**

These models are managed through a centralized `SNNModelManager` class, which can load, run, and manage multiple models.

## File Structure

```plaintext
├── model_base.py         # Contains the base abstract class for SNN models
├── spiking_manager.py    # Contains the SNNModelManager class for managing multiple models
├── spiking_resnet.py     # Contains the SpikingResNet class
├── spiking_vgg.py        # Contains the SpikingVGG class
├── main.py               # Main script to run and test models
├── data_loader.py        # Contains the base code for loading data
├── demos                 # Main folder to run and test our library
  ├── load_cifar.py       # Main notebook to load and visualize CIFAR10 dataset
├── requirements.txt      # Contains the dependencies needed to run code
└── README.md             # Project documentation
```

## Installation

Certain dependencies are required to run this library. Install them with conda using: `conda create --name <env> --file requirements.txt` 


