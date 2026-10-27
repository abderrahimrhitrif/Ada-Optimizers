# Ada Optimizers from Scratch

## Overview
This project provides from-scratch implementations and comparative experiments of various Adaptive Gradient Optimization algorithms (such as AdaGrad) implemented purely in Python and NumPy. It explores their convergence characteristics, gradient accumulation dynamics, and empirical performance on the MNIST digit classification dataset.

## Architecture & Implementation
- **Mathematical Implementations**: Pure NumPy implementations of adaptive gradient update equations, incorporating parameters such as learning rate ($lpha$), smoothing epsilon ($\epsilon$), and accumulated squared gradients ($G$).
- **Data Pipeline**: Direct download and loading of the MNIST dataset (`mnist.npz`) via NumPy array manipulation without relying on heavy deep learning frameworks.
- **Optimization Loops**: Custom training loops calculating forward pass, loss computation, gradient derivation, and parameter updates step-by-step.

## Data
- **Dataset**: MNIST handwritten digits dataset (`mnist.npz`).
- **Processing**: Direct NumPy loading and feature normalization.

## Method & Algorithms
- **AdaGrad / Adaptive Updates**: Dynamically scales learning rates per parameter inversely proportional to the square root of historical squared gradients.
- **Gradient Derivation**: Explicit calculation of analytical gradients for custom loss formulations and matrix operations.

## Verified Results & Metrics
- Successfully executed training loops and verified step-wise reduction in loss over epochs on subset tasks and MNIST data.

## Limitations & Caveats
- Educational and experimental implementations; not optimized as a production deep learning library.
- Relies on simple feedforward or custom scalar loss functions in initial script cells before full MNIST integration.

## Run Instructions
```bash
jupyter notebook Ada.ipynb
```
