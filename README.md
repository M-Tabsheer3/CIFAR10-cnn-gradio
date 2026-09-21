# CIFAR-10 Image Classifier (CNN + Gradio)

A Convolutional Neural Network that classifies images into 10 categories, deployed as an interactive web app using Gradio.

Built as part of the Data Science program at **NED Academy, NED University of Engineering and Technology**.

## Overview

- **Task:** Multi-class image classification
- **Dataset:** CIFAR-10 (60,000 32x32 color images, 10 classes)
- **Framework:** TensorFlow / Keras
- **Deployment:** Gradio
- **Environment:** Google Colab (T4 GPU)
- **Test Accuracy:** 74.44%

## Classes

`airplane` `automobile` `bird` `cat` `deer` `dog` `frog` `horse` `ship` `truck`

## Model Architecture

- 3 convolutional blocks (Conv2D + BatchNormalization + MaxPooling)
- Dropout layers for regularization
- Data augmentation (random flip, rotation, zoom)
- Dense classifier with softmax output
- Optimizer: Adam | Loss: Sparse Categorical Crossentropy
- EarlyStopping to prevent overfitting

## Results

| Metric | Value |
|---|---|
| Test Accuracy | 74.44% |

Accuracy/loss curves, the classification report, and the confusion matrix are available in the notebook.

## Web App Features

- Upload any image and get instant predictions
- Top 3 predicted classes with confidence scores
- Sample images to try
- Clean, classic interface built with Gradio Blocks

## Project Structure

```
├── cifar10_gradio.ipynb     # Data loading, model training, evaluation, Gradio app
└── README.md
```

## How to Run

1. Open the notebook in [Google Colab](https://colab.research.google.com/).
2. Go to **Runtime → Change runtime type → T4 GPU**.
3. Run all cells from top to bottom (**Runtime → Run all**).
4. The last cell launches the Gradio app and prints a public link.

## Tech Stack

Python, TensorFlow/Keras, NumPy, Pillow, Matplotlib, Seaborn, scikit-learn, Gradio

## Limitations

CIFAR-10 images are 32x32, so uploaded images are resized down. Predictions work best on clear, centered images of the 10 supported classes.

## Acknowledgements

- Instructor: **Sir Sajid Majeed**
- Focal Person: **Sir Najeed Ahmed Khan**
- NED Academy, NED University of Engineering and Technology

## Author

**Muhammad Tabsheer**
[GitHub](https://github.com/M-Tabsheer3) | [LinkedIn](https://linkedin.com/in/muhammad-tabsheer-6a273a27a/) | [Portfolio](https://M-Tabsheer3.github.io)
