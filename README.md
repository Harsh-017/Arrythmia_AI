# Arrhythmia AI - AI-Powered ECG Disease Detection

Arrhythmia AI is an AI-based system designed to detect heart diseases using Electrocardiogram (ECG) data. It utilizes a convolutional neural network (CNN) to classify ECG signals and identify potential arrhythmias and other heart-related conditions.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Libraries Used](#libraries-used)
- [Installation](#installation)
- [Usage](#usage)
- [Model Information](#model-information)
- [GUI Functionality](#gui-functionality)
- [Example Code Snippet](#example-code-snippet)
- [Contributing](#contributing)
- [License](#license)

## Overview
Arrhythmia AI enables users to analyze ECG data and leverages a CNN model to detect abnormalities such as arrhythmias. This application simplifies the process of diagnosing heart conditions using AI.

## Features
- Detect heart diseases using ECG data.
- CNN-based heart disease classification.
- User-friendly GUI for uploading images of different arrhythmias.

## Tech Stack
- **Backend**: Python, TensorFlow, Keras
- **Database**: MIT-BIH Arrhythmia Database (for model training)
- **GUI Framework**: Tkinter

## Libraries Used
The following libraries are utilized in the Arrhythmia AI project:

- tkinter: For creating the GUI.
- PIL: For image processing.
- numpy: For numerical operations.
- keras: For loading and using the deep learning model.

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/Arrhythmia-AI.git
   cd Arrhythmia-AI

2. **Create and activate a virtual environment:**
   ```bash
   python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate


3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   
## Usage
- **Upload ECG Data**: Users can upload images of different types of arrhythmias through the GUI.
- **View Results**: The model will analyze the uploaded images and provide predictions regarding the type of arrhythmia detected.

## Model Information
- **Model**: Convolutional Neural Network (CNN)
- **Dataset**: MIT-BIH Arrhythmia Database
- **Training Accuracy**: 98%
- **Validation Accuracy**: 95%

The CNN model was trained on ECG data from the MIT-BIH Arrhythmia Database to detect multiple types of heart diseases. The model architecture includes multiple convolutional layers to extract features from ECG waveforms, followed by fully connected layers for classification.

## GUI Functionality
The GUI for Arrhythmia AI allows users to:
- Upload an image of an ECG signal.
- The uploaded image is displayed in the interface.
- Once an image is uploaded, the user can click a "Detect Image" button to trigger the model's prediction.
- The model will classify the uploaded image and display whether it is "Uninfected" or provide a diagnosis if it detects an arrhythmia.

## Example Code Snippet
```python
import tkinter as tk
from tkinter import filedialog
from tkinter import *
from PIL import Image, ImageTk
import numpy as np
from keras.models import load_model

# Initialising GUI
top = tk.Tk()
top.geometry('800x600')
top.title('Heart Disease Detection')
top.configure(background='#F0E68C')

# Loading the model
model = load_model('model_vgg19.h5')

# Function to detect heart disease
def detect(file_path):
    # [Detection logic here]

# Function to show detect image button
def show_detect_buttons(file_path):
    # [Button logic here]

# Function to upload image
def upload_image():
    # [Upload logic here]

# GUI components
# [GUI components setup here]

top.mainloop()

```


## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-name`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature-name`).
5. Open a Pull Request.

## License
This project is licensed under the MIT License - see the LICENSE file for details.



