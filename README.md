# Convolutional Neural Network for Brain Tumor Classification

This repository contains a Python notebook implementing a Convolutional Neural Network (CNN) using TensorFlow and Keras to classify brain MRI images into four categories.

## Features

- Loads and preprocesses a curated brain MRI dataset
- Builds a CNN using Keras Sequential API
- Trains and evaluates the model
- Visualizes training history (accuracy and loss)
- Generates and displays a confusion matrix for evaluation

## Dataset

The dataset used in this project is a curated combination of three publicly available sources:

1. **Figshare**  
2. **SARTAJ Dataset**  
3. **Br35H Dataset**

It contains a total of **7,023 MRI images** of the human brain, categorized into four classes:

- **Glioma**
- **Meningioma**
- **Pituitary**
- **No Tumor**

### Important Notes on Dataset Curation

- The images in the **"No Tumor"** class were sourced from the **Br35H** dataset.
- The **SARTAJ dataset** was found to have miscategorized images in the **"Glioma"** class. Based on observations from various models and results reported by other researchers, these misclassifications were confirmed.
- As a corrective step, all glioma images from the SARTAJ dataset were removed and replaced with accurately labeled images from the **Figshare** dataset.

This preprocessing was done to ensure higher data quality and model reliability.

## Model Architecture

The CNN consists of:

- Convolutional layers with ReLU activation
- MaxPooling layers to reduce feature dimensions
- Dropout layers for regularization
- Fully connected (Dense) layers for classification
- Softmax activation for multiclass prediction

## Getting Started

### Prerequisites

Install the necessary Python libraries:

```bash
pip install tensorflow matplotlib seaborn scikit-learn
```



## Files

- `CNN.ipynb`: Main notebook implementing the CNN model
- `README.md`: Project overview and setup guide

## Contact

For questions, feedback, or contributions, feel free to open an issue or submit a pull request.
