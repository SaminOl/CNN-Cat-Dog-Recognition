# CNN Cat-Dog Image Classifier

This repository contains a Convolutional Neural Network (CNN) model developed to classify images of cats and dogs. The project demonstrates a fundamental application of deep learning for image recognition using TensorFlow/Keras.

## Table of Contents

-   [Project Overview](#project-overview)
-   [Features](#features)
-   [Installation](#installation)
-   [Dataset](#dataset)
-   [Usage](#usage)
-   [Model Architecture](#model-architecture)
-   [Results](#results)
-   [Future Work](#future-work)
-   [License](#license) (Optional)

## Project Overview

This project implements a CNN from scratch to accurately distinguish between images of cats and dogs. It covers data loading, preprocessing (including data augmentation), model definition, training, and evaluation. The goal is to showcase how CNNs leverage spatial hierarchies of patterns to achieve high performance in image classification tasks.

## Features

-   **Image Preprocessing:** Images are resized and normalized.
-   **Data Augmentation:** Utilizes `ImageDataGenerator` for rotations, flips, and zooms to enhance model robustness and prevent overfitting.
-   **CNN Architecture:** A sequential model with multiple `Conv2D` and `MaxPool2D` layers for hierarchical feature extraction.
-   **Model Training:** Trained using the Adam optimizer and categorical cross-entropy loss.
-   **Performance Evaluation:** Reports accuracy, a detailed classification report (precision, recall, F1-score), and a confusion matrix.

## Installation

To set up the project locally, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/SaminOl/CNN-Cat-Dog-Recognition.git](https://github.com/SaminOl/CNN-Cat-Dog-Recognition.git)
    cd CNN-Cat-Dog-Recognition
    ```

2.  **Create a virtual environment (recommended):**
    Using a virtual environment helps manage project dependencies.
    ```bash
    python -m venv venv
    # On Windows:
    .\venv\Scripts\activate
    # On macOS/Linux:
    source venv/bin/activate
    ```

3.  **Install required Python libraries:**
    ```bash
    pip install tensorflow numpy matplotlib seaborn scikit-learn opencv-python
    ```
    (Note: `opencv-python` is for `cv2` operations if used elsewhere in your project, e.g., for single image testing.)

## Dataset

This project utilizes the `cat_dog_2.zip` dataset. **This dataset is NOT included in this repository due to its large size.**

You can download the dataset from [**INSERT LINK TO DATASET SOURCE HERE (e.g., your Google Drive link, Kaggle, etc.)**].

After downloading, please unzip the file into a `Datasets` folder (e.g., `D:\Computer vision\Files\Datasets\`) such that the directory structure matches the one expected by the `ImageDataGenerator`:
