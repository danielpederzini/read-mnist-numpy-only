# MNIST Digit Classifier - Neural Network from Scratch
A deep learning project implementing a neural network **from scratch using only NumPy** to classify hand-written digits from the MNIST dataset. This project demonstrates core machine learning concepts including forward propagation, backpropagation, and gradient descent.

## Project Overview
This repository showcases the implementation of a 3-layer neural network without relying on high-level frameworks like TensorFlow or PyTorch. The network successfully learns to recognize hand-written digits with competitive accuracy.

## Architecture
- **Input Layer**: 784 neurons (28×28 pixel images flattened)
- **Hidden Layer 1**: 64 neurons with ReLU activation
- **Hidden Layer 2**: 64 neurons with ReLU activation
- **Output Layer**: 10 neurons with Softmax activation (one per digit class 0-9)

**Forward Pass**: Input → Linear → ReLU → Linear → ReLU → Linear → Softmax → Output

**Weight Initialization**: He initialization (scaled by √(2/fan_in)) for ReLU layers and Xavier initialization for output layer

**Loss Function**: Cross-entropy loss with categorical targets

## Key Features
- Pure NumPy implementation (no deep learning frameworks)
- Complete backpropagation algorithm from scratch
- Proper weight initialization using He/Xavier methods for stable training
- Training and evaluation on full MNIST dataset (60,000 training + 10,000 test samples)
- Comprehensive visualizations:
  - Learned features from both hidden layers side-by-side
  - Activation maps from all layers for sample predictions
  - Output probability distributions with prediction indicators

## Technologies Used
- **NumPy**: Core numerical computations
- **Matplotlib**: Data visualization
- **Python 3**: Language

## Dataset
- **MNIST**: 70,000 images of hand-written digits (28×28 pixels)
- **Training Set**: 60,000 images
- **Test Set**: 10,000 images
- **Normalization**: Pixel values scaled to [0, 1]

## Results
The model learns meaningful representations:
- Loss decreases over epochs
- Test accuracy improves with training
- Hidden layer weights visualize interpretable digit features (shown in the final visualizations)

<img width="1585" height="789" alt="weights" src="https://github.com/user-attachments/assets/6a639950-b2e6-43e0-b631-195af614f54b" />
<img width="1389" height="3189" alt="predictions" src="https://github.com/user-attachments/assets/8052dfa5-09fb-40c5-8c0c-ce68e86a3fa2" />

## How to Run

### Prerequisites
```bash
pip install numpy matplotlib
```

### Usage
1. Clone the repository
2. Run the Jupyter notebook: `main.ipynb`
3. Monitor the average loss and test accuracy after each epoch to track training progress.

**Author**: Daniel Pederzini  
**Purpose**: Deep Learning Educational Project
