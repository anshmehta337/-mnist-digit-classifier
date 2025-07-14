# -mnist-digit-classifier
# MNIST Digit Classifier

A neural network built with TensorFlow and Keras to classify handwritten digits from the MNIST dataset. The model achieves up to 97.6% accuracy using a simple feedforward architecture and optimized data preprocessing.

---

## Overview

- Dataset: MNIST handwritten digits (28x28 grayscale images)
- Framework: TensorFlow / Keras
- Environment: Google Colab
- Model Type: Fully connected neural network
- Accuracy: 97.6%

---

## Files

- `mnist_digit_classifier.ipynb` – Full implementation in Colab
- `confusion_matrix.png` – Heatmap of classification results (optional)

---

## Model Architecture

- Input layer: 784 nodes (flattened 28x28 image)
- Hidden layer: 100 neurons, ReLU activation
- Output layer: 10 neurons, Softmax activation
- Optimizer: Nadam
- Loss function: Sparse categorical crossentropy

---

## Preprocessing Techniques Tested

| Method           | Accuracy |
|------------------|----------|
| StandardScaler   | ~96.1%   |
| MinMaxScaler     | 97.6%    |

MinMaxScaler outperformed StandardScaler, likely due to its ability to preserve the 0–255 pixel intensity scale by normalizing to [0, 1].

---

## Results

- Final test accuracy: **97.6%**
- Loss: 0.0737
- Confusion matrix heatmap generated for visual analysis

---

## How to Run

1. Open the notebook in Google Colab.
2. Run all cells to train and evaluate the model.
3. View performance metrics and visualization outputs.

---

## Future Improvements

- Add validation accuracy tracking
- Visualize misclassified examples
- Try CNN for even higher accuracy
- Deploy using Streamlit or Flask for live predictions

---

## Author

[Ansh Mehta](https://github.com/anshmehta337)

