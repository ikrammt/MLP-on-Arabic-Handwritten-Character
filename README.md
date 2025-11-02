# Arabic Handwritten Character Recognition (MLP)

This project implements a **Multilayer Perceptron (MLP)** to recognize **Arabic handwritten characters** using the **Arabic Handwritten Characters Dataset (AHCD)**. The model is built **from scratch using NumPy**, without deep learning frameworks.

## 📦 Dataset
The dataset consists of grayscale handwritten Arabic letters:
- **Training set:** 13,440 images
- **Test set:** 3,360 images
- Each image is **32×32 → 1024 pixels**
- Labels range from **1 to 28**, each representing one Arabic character.

Pixel values are normalized to the range **[0.01, 0.99]** before training.

## 🧠 Model Architecture

| Layer | Size | Activation |
|------|------|------------|
| Input Layer | 1024 | - |
| Hidden Layer 1 | 512 | ReLU |
| Hidden Layer 2 | 256 | ReLU |
| Hidden Layer 3 | 128 | ReLU |
| Output Layer | 28 classes | Softmax |

