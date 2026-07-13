# Image-Classification

This repository contains a Python script for classifying images using a pre-trained Keras model. It loads an image, preprocesses it, and then uses the model to predict the class and confidence score.

## Table of Contents
- [Features](#features)
- [Requirements](#requirements)
- [Setup](#setup)
- [Usage](#usage)
- [Example Output](#example-output)

## Features
- Loads a pre-trained Keras H5 model for image classification.
- Preprocesses images by resizing, cropping, and normalizing.
- Predicts the class and confidence score of an input image.

## Requirements
- Python 3.x
- TensorFlow (or `tf_keras` if using TensorFlow 2.16+)
- Pillow (PIL)
- NumPy

## Setup

1.  **Clone the repository (or copy the code):**
    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```

2.  **Install dependencies:**
    ```bash
    pip install tensorflow numpy pillow tf_keras # Use tf_keras if you're on a newer TensorFlow version
    ```

3.  **Obtain the pre-trained model and labels:**
    -   Place your Keras model file named `keras_model.h5` in the same directory as the script.
    -   Place your labels file named `labels.txt` (each label on a new line) in the same directory.

    *Note: The example assumes a model trained with image dimensions 224x224 and RGB channels.* 

## Usage

1.  **Prepare your image:**
    -   Make sure your input image is accessible. The example uses `/content/images (12).jpg`.

2.  **Run the script:**
    Open a Python environment (like Google Colab or your local machine) and execute the code. You will need to replace the image path with your desired image.

    Modify the line:
    ```python
    image = Image.open("/content/images (12).jpg").convert("RGB")
    ```
    to point to your image file.

3.  **Output:**
    The script will print the predicted class and its confidence score.

## Example Output

1/1 [==============================] - 2s 2s/step Class: Rabbit Confidence Score: 0.98954016
