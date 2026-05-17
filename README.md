# CNN-CIFAR10-PyTorch

Convolutional Neural Network implemented in PyTorch for image classification on the CIFAR-10 dataset.

## Features

- Deep CNN architecture with 8 convolutional layers
- CIFAR-10 image classification
- GPU training support with CUDA
- TensorBoard integration for monitoring loss and accuracy
- Training and validation pipelines implemented from scratch
- SGD optimizer with momentum and L2 regularization

## Technologies

- Python
- PyTorch
- TensorBoard
- CUDA
- NumPy
- Matplotlib

## Model Architecture

| Layer | Output Shape |
|------|------|
| Conv2D (32 filters) | 30x30x32 |
| Conv2D (64 filters) | 28x28x64 |
| Conv2D (128 filters) | 26x26x128 |
| MaxPooling | 13x13x128 |
| Conv2D (256 filters) | 11x11x256 |
| Conv2D (512 filters) | 9x9x512 |
| MaxPooling | 3x3x512 |
| Conv2D (1024 filters) | 1x1x1024 |
| Fully Connected | 100 |
| Output Layer | 10 |

## Results

- Trained for 50 epochs
- Achieved approximately 72% validation accuracy on CIFAR-10
- Observed overfitting after ~30 epochs during training

## Run

Install dependencies:

```bash
pip install -r requirements.txt
```