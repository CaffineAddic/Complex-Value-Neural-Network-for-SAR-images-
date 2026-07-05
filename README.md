# Complex-Valued Neural Networks for Polarimetric SAR Image Classification

> Deep learning framework for Polarimetric Synthetic Aperture Radar (PolSAR) image classification using Complex-Valued Neural Networks.

[![Python](https://img.shields.io/badge/Python-3-blue)](#)
[![PyTorch](https://img.shields.io/badge/PyTorch-Deep%20Learning-red)](#)
[![Research](https://img.shields.io/badge/Status-Research-success)](#)

This repository investigates the application of **Complex-Valued Neural Networks (CVNNs)** to Polarimetric Synthetic Aperture Radar (PolSAR) image classification. Unlike conventional neural networks that process only real-valued inputs, CVNNs preserve the amplitude and phase information naturally present in SAR measurements, allowing the model to learn directly from the complex-valued scattering matrix.

The work was completed as part of my undergraduate research internship and explores whether complex-valued architectures provide improved representation learning for remote sensing applications.

---

## Overview

Polarimetric SAR sensors measure both the magnitude and phase of electromagnetic backscatter, producing inherently complex-valued observations.

Traditional deep learning approaches often discard the phase component by converting complex data into separate real-valued channels. This repository instead investigates end-to-end learning using complex-valued neural networks that preserve the physical characteristics of the measured signal.

The implementation focuses on land-cover classification using PolSAR imagery.

---

## Methodology

The workflow consists of:

1. Preprocessing complex-valued PolSAR datasets.
2. Feature extraction from scattering matrix representations.
3. Construction of complex-valued neural network layers.
4. Supervised training for land-cover classification.
5. Performance evaluation against conventional approaches.

The implementation explores:

- Complex-valued convolutions
- Complex activation functions
- Complex batch normalisation
- Complex-valued optimisation

---

## Features

- Complex-valued neural network implementation
- Polarimetric SAR image processing
- End-to-end classification pipeline
- PyTorch implementation
- Experimental evaluation on remote sensing datasets

---

## Repository Structure

```text
.
├── notebooks/
├── datasets/
├── models/
├── training/
├── evaluation/
├── figures/
└── README.md
```

---

## Installation

Clone the repository

```bash
git clone https://github.com/CaffineAddic/Complex-Value-Neural-Network-for-SAR-images-.git
cd Complex-Value-Neural-Network-for-SAR-images-
```

Install the required packages

```bash
pip install -r requirements.txt
```

or

```bash
pip install torch torchvision numpy scipy matplotlib jupyter
```

---

## Usage

Launch Jupyter Notebook

```bash
jupyter notebook
```

The notebooks cover:

- dataset preparation
- preprocessing
- model training
- evaluation
- visualisation

---

## Results

The repository demonstrates the implementation of complex-valued deep learning techniques for PolSAR classification while preserving both amplitude and phase information throughout the learning pipeline.

The accompanying report discusses the architectural design, implementation details, and experimental observations.

---

## Background

Complex-valued neural networks are particularly well suited to SAR processing because radar measurements are naturally represented in the complex domain. Preserving phase information enables models to exploit physical characteristics that may be lost when using purely real-valued representations.

---

## Related Work

This project complements my work on:

- Laser absorption spectroscopy using Gaussian Processes
- Wavelet analysis of combustion diagnostics
- Meta-learning with MAML and FOMAML

---

## Author

**Saumya Roy**

---

## License

GNU General Public License v3.0
