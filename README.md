# Handwritten Digit Recognizer — Neural Network from Scratch

A simple neural network built from scratch using only NumPy to classify handwritten digits from the MNIST dataset. No deep learning frameworks (no TensorFlow, no PyTorch) — just math and NumPy.

## Results
- **Training accuracy: ~90%** after 500 iterations
- Dataset: [Kaggle Digit Recognizer](https://www.kaggle.com/competitions/digit-recognizer)

## Network Architecture
Input Layer → Hidden Layer → Output Layer
784 nodes      10 nodes      10 nodes
(28x28px)      (ReLU)       (Softmax)
## How It Works

**Forward Propagation:**
- Input: flattened 28×28 pixel image (784 features), normalized to [0, 1]
- Hidden layer: linear transformation + ReLU activation
- Output layer: linear transformation + Softmax activation → probability per digit

**Backward Propagation:**
- Loss: cross-entropy
- Optimizer: gradient descent
- Weight initialization: He initialization (ideal for ReLU)
