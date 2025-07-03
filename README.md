# Malaria Cell Classification using Convolutional Neural Networks

This repository contains code for building and training a Convolutional Neural Network (CNN) to classify malaria cells as infected or uninfected. The model is trained on the Malaria dataset available in TensorFlow Datasets.

## Dataset
The Malaria dataset used in this project contains images of cells infected and uninfected with the malaria parasite. The dataset is split into training, validation, and test sets.

## Installation
1. Clone the repository
2. Install the required libraries

## Usage
1. Run the `malaria_cell_classification.ipynb` notebook to train the model and evaluate its performance.
2. You can modify the hyperparameters, model architecture, or preprocessing steps as needed.
3. Use the trained model for inference by loading it from the saved file (`malaria_model.keras`) and passing new images.

## Model Architecture
The CNN model architecture used for this classification task is as follows:
- Input: 120x120x3 image
- Convolutional Layer 1: 64 filters, kernel size 3x3, ReLU activation
- Max Pooling Layer 1: Pool size 2x2
- Convolutional Layer 2: 128 filters, kernel size 3x3, ReLU activation
- Max Pooling Layer 2: Pool size 2x2
- Batch Normalization Layer
- Flatten Layer
- Dense Layer: 128 units, ReLU activation
- Output Layer: 1 unit, Sigmoid activation

## Results
- The model achieved an accuracy of 80% on the test dataset.
- Training and validation loss/accuracy curves are visualized in the notebook.

## Acknowledgments
- The Malaria dataset is available in TensorFlow Datasets.
- Inspiration and guidance from various online tutorials and resources.
