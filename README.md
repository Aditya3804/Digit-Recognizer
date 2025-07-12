# Digit-Recognizer

# 🧠 Handwritten Digit Classifier using CNN

This project builds a Convolutional Neural Network (CNN) to classify handwritten digits (0–9) using the MNIST dataset. The model achieves over **97% accuracy** and includes performance graphs, a confusion matrix, and saved model support.

---

## 📦 Dataset

- **MNIST**: 70,000 grayscale 28x28 pixel images of digits
- 60,000 for training, 10,000 for testing
- Automatically loaded via TensorFlow

---

## 🧱 Model Architecture

```text
Input: 28x28x1
↓
Conv2D(64 filters, 3x3) → ReLU
↓
MaxPooling2D(2x2) 
↓
Conv2D(64 filters, 3x3) → ReLU
↓
MaxPooling2D(2x2)
↓
Flatten → Dense(128) → ReLU → Dropout(0.5)
↓
Dense(10) → Softmax
