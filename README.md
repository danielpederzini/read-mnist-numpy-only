# MNIST Digit Classifier - Neural Network from Scratch
A deep learning project implementing a neural network **from scratch using only NumPy** to classify hand-written digits from the MNIST dataset. This project demonstrates core machine learning concepts including forward propagation, backpropagation, and gradient descent.

## Project Overview
This repository showcases the implementation of a 2-layer neural network without relying on high-level frameworks like TensorFlow or PyTorch. The network successfully learns to recognize hand-written digits with competitive accuracy.

## Architecture
- **Input Layer**: 784 neurons (28×28 pixel images flattened)
- **Hidden Layer**: 128 neurons with ReLU activation
- **Output Layer**: 10 neurons with Softmax activation (one per digit class 0-9)

**Forward Pass**: Input → Linear → ReLU → Linear → Softmax → Output

**Loss Function**: Cross-entropy loss with categorical targets

## Key Features
- Pure NumPy implementation (no deep learning frameworks)
- Complete backpropagation algorithm from scratch
- Training and evaluation on full MNIST dataset (60,000 training + 10,000 test samples)
- Visualization of learned hidden layer features and full network flow

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

<img width="1326" height="660" alt="weights" src="https://github.com/user-attachments/assets/34e1df9c-83fe-495f-b02a-bfcc253dc69b" />
<img width="1354" height="1589" alt="predictions" src="https://github.com/user-attachments/assets/784e1c95-7e51-4721-9e57-a9e3ab0a2edd" />

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
