# Handwritten Digit Recognition with MNIST

This project demonstrates a basic deep learning model using TensorFlow and Keras to classify handwritten digits from the MNIST dataset. It also includes functionality to predict digits from custom images.

## Features

- Trains a neural network on the MNIST dataset
- Saves and loads the trained model
- Evaluates model accuracy on test data
- Uses OpenCV to preprocess and predict digits from user-provided images
- Displays predictions with Matplotlib

## Requirements

Install dependencies using pip:

```bash
pip install tensorflow numpy opencv-python matplotlib
```

## Dataset
The model is trained on the MNIST dataset, which is automatically downloaded via TensorFlow's dataset loader.

## Training the Model

The model consists of:
- Input layer: Flattened 28x28 image
- Two hidden layers with 128 neurons and ReLU activation
- Output layer with 10 neurons and softmax activation

## To train and save the model:

```bash
python your_script.py
```

## Predicting Custom Digits
Place PNG images named digit1.png, digit2.png, ..., in a digits/ folder. Each image should:
- Be 28x28 pixels
- Have a dark digit on a light background

## The script will:
- Load each image
- Invert pixel values
- Predict the digit using the trained model
- Display the image and predicted value

## Output Example
```
This digit is probably a 7
This digit is probably a 2
```
