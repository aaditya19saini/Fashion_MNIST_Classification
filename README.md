# Fashion MNIST Classification

A neural network classifier for the [Fashion MNIST](https://github.com/zalandoresearch/fashion-mnist) dataset built with TensorFlow/Keras.

## Overview

This project trains a fully connected neural network to classify 28×28 grayscale images of clothing items into 10 categories:

| Label | Class |
|-------|-------|
| 0 | T-shirt/top |
| 1 | Trouser |
| 2 | Pullover |
| 3 | Dress |
| 4 | Coat |
| 5 | Sandal |
| 6 | Shirt |
| 7 | Sneaker |
| 8 | Bag |
| 9 | Ankle boot |

## Model Architecture

| Layer | Units | Activation |
|-------|-------|------------|
| Input | 28×28 | — |
| Flatten | 784 | — |
| Dense | 300 | ReLU |
| Dense | 100 | ReLU |
| Dense (output) | 10 | Softmax |

- **Loss function:** Sparse Categorical Crossentropy
- **Optimizer:** SGD
- **Epochs:** 50

## Dataset Split

| Set | Samples |
|-----|---------|
| Training | 55,000 |
| Validation | 5,000 |
| Test | 10,000 |

All pixel values are normalized to the [0, 1] range.

## Results

- **Test Accuracy:** ~87–89%
- **Test Loss:** ~0.35–0.50

Training and validation loss/accuracy curves are plotted in the notebook for visual inspection.

## Requirements

- Python 3.x
- TensorFlow
- NumPy
- Pandas
- Matplotlib

## Usage

Open `fashion_mnist.ipynb` in Jupyter Notebook or VS Code and run all cells sequentially.

```bash
pip install tensorflow numpy pandas matplotlib
```
