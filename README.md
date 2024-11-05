# MNIST Handwritten Digit Classification

This project implements a neural network model to classify handwritten digits from the MNIST dataset using TensorFlow and Keras. The workflow includes data preparation, model building, training, evaluation, and visualization of results.

### Data Preparation
- The MNIST dataset is loaded and split into training and test sets.
- Labels are one-hot encoded to prepare them for classification tasks.
- Input images are reshaped to have a single channel (28x28x1) and standardized to float values in the range [0, 1].

### Modeling
A sequential neural network is constructed with the following architecture:
- **Input Layer**: Flatten layer converting the 2D images into a 1D array.
- **Hidden Layer**: Dense layer with 128 units and ReLU activation function.
- **Output Layer**: Dense layer with 10 units (for 10 classes) and softmax activation.

The model is compiled using categorical crossentropy as the loss function, Adam optimizer, and metrics for precision, recall, and accuracy.

### Training and Evaluation
- The model is trained for 10 epochs with a batch size of 128, utilizing the training data and validating on the test set.
- The training history is logged to analyze performance over epochs.

### Results Visualization
- Accuracy and loss are plotted to visualize the model’s performance on both training and validation datasets.

## Results
- The model achieves high accuracy, with the training accuracy reaching above 99% after 10 epochs.
- Loss values decrease steadily, indicating effective learning.

## Requirements
- Python 3.x
- TensorFlow
- Keras
- Matplotlib
- NumPy
