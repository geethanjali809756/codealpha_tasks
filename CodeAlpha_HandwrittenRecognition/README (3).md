# Handwritten Character Recognition

A deep learning project to recognize handwritten digits and alphabets using Convolutional Neural Networks (CNN), developed as part of the **CodeAlpha Machine Learning Internship**.

---

## Overview

This project covers recognition of handwritten characters in two parts — **digits (0–9)** using the MNIST dataset and **letters (A–Z)** using the EMNIST Letters dataset. Both use the same CNN architecture trained independently with data augmentation for better generalization.

---

## Datasets

| Part | Dataset | Classes | Training Samples |
|------|---------|---------|-----------------|
| Digits | MNIST (Keras built-in) | 0–9 (10 classes) | 60,000 |
| Letters | EMNIST Letters (auto-downloaded) | A–Z (26 classes) | ~88,800 |

No manual download required — all datasets load automatically when the notebook runs.

---

## Technologies Used

- Python, NumPy, Pandas
- Matplotlib, Seaborn, OpenCV
- TensorFlow / Keras
- Google Colab (GPU recommended)

---

## Model Architecture

CNN with 3 Convolutional Blocks followed by Fully Connected layers:

- Conv2D → BatchNormalization → Conv2D → MaxPooling → Dropout
- Conv2D → BatchNormalization → Conv2D → MaxPooling → Dropout
- Conv2D → BatchNormalization → MaxPooling → Dropout
- Dense (256) → BatchNormalization → Dropout → Output (Softmax)

---

## Project Workflow

1. Load datasets (MNIST via Keras, EMNIST via package)
2. Preprocess — normalize, reshape, fix orientation
3. Data augmentation (rotation, shift, zoom)
4. Build and train CNN model
5. Evaluate with accuracy, confusion matrix, classification report
6. Predict on custom handwritten images
7. Save trained models as `.h5` files

---

## Evaluation Metrics

Models are evaluated using Accuracy, Confusion Matrix, and Classification Report (Precision, Recall, F1 Score per class).

---

## Getting Started

```bash
# Install dependencies
pip install tensorflow numpy pandas matplotlib seaborn opencv-python emnist
```

Open the notebook in Google Colab, enable GPU (Runtime → Change runtime type → T4 GPU), and run all cells sequentially.

---

## Repository Structure

```
CodeAlpha_HandwrittenRecognition/
├── CodeAlpha_HandwrittenRecognition.ipynb
├── README.md
└── models/
    ├── mnist_digit_model.h5
    └── emnist_letter_model.h5
```

---

## Outcome

The project successfully recognizes handwritten digits and letters using a CNN model. Custom handwritten images can be uploaded directly in Colab for real-time prediction using the built-in `predict_digit()` and `predict_letter()` functions.

---

## Author

**Geethanjali**  
CodeAlpha Machine Learning Internship
