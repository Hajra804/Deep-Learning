# Deep-Learning
# Deep Learning for Perception 

## Building, Breaking and Fixing a Neural Network

This repository contains our implementation and experimental results for
Assignment 01 of Deep Learning for Perception.

The assignment focuses on understanding neural networks by implementing,
training, evaluating, breaking, and improving different neural network
configurations.

---

## Dataset

We use the **Fashion-MNIST** dataset from Zalando Research.

The dataset contains grayscale images of clothing items belonging to
10 different classes.

### Preprocessing

- Pixel values are normalized to the range `[0, 1]`.
- Each `28 × 28` image is flattened into a `784`-dimensional vector.
- The provided training data is divided into:
  - 80% training data
  - 20% validation data
- The test set is kept separate and is evaluated only in Part 7.

### Classes

| Label | Class |
|------:|-------|
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

---

## Environment

The experiments were performed using:

- Python
- Kaggle Notebook
- GPU: NVIDIA T4
- NumPy
- PyTorch
- Pandas
- Matplotlib
- Scikit-learn

---

# Assignment Parts

## Part 1 — Neural Network from Scratch

A two-layer multilayer perceptron was implemented using NumPy.

### Architecture

```text
Input: 784
   ↓
Hidden Layer: 64 neurons
   ↓
ReLU
   ↓
Output: 10 neurons
   ↓
Softmax
