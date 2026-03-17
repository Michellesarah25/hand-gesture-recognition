# hand-gesture-recognition
![Python](https://img.shields.io/badge/Python-3.8+-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange)
![Status](https://img.shields.io/badge/Status-Complete-green)
CNN-based hand gesture classifier using LeapGestRecog dataset on kaggle

# Hand Gesture Recognition using Deep Learning

A Computer Vision project that classifies human hand gestures 
from images using a Convolutional Neural Network (CNN).

## Overview
This project builds an end-to-end deep learning pipeline to 
recognize and classify hand gestures using the 
[LeapGestRecog dataset](https://www.kaggle.com/datasets/gti-upm/leapgestrecog) 
from Kaggle. The trained model can identify gestures such as 
fist, palm, thumb, and more — with potential applications in 
touchless computer control systems.

## Dataset
- **Source:** [LeapGestRecog — Kaggle](https://www.kaggle.com/datasets/gti-upm/leapgestrecog)
- **Classes:** palm, fist, thumb, index, palm_moved, down
- **Input size:** 128×128 grayscale images

## Model Architecture
- Conv2D (32 filters) → BatchNormalization → MaxPooling
- Conv2D (64 filters) → BatchNormalization → MaxPooling
- Conv2D (128 filters) → BatchNormalization → MaxPooling
- Flatten → Dense (256) → Dropout (0.5)
- Output: Softmax (multi-class classification)
- **Total Parameters:** ~6.4 million

## Tech Stack
- Python
- TensorFlow / Keras
- NumPy, Matplotlib
- Google Colab

## Features
- ImageDataGenerator for real-time data augmentation
  (rotation, zoom, flip, shift)
- EarlyStopping and ModelCheckpoint callbacks
- Training/validation accuracy and loss visualization
- Random test image prediction with visual output
- Model saved as `best_model.h5` for deployment

## Results
- Trained over 25 epochs using Adam optimizer
- Monitored validation accuracy with early stopping
- Accuracy and loss curves plotted for analysis

## How to Run
1. Download [LeapGestRecog dataset](https://www.kaggle.com/datasets/gti-upm/leapgestrecog) from Kaggle
2. Upload dataset to your Google Colab environment
3. Open the notebook → [Run in Google Colab](https://colab.research.google.com/drive/100BWqNwuYtK98ldsn13sl1hWNyfYws2j)
4. Run all cells sequentially
5. Model saves automatically as `best_model.h5`

## Future Scope
- Real-time gesture recognition via webcam
- Integration with computer control applications
  (e.g., volume control by waving hand)
- Improved accuracy with transfer learning

## Author
**Michelle Sarah David**  
Final Year B.Tech — AI & Data Science  
Sri Venkateswara College of Engineering, Chennai  
[LinkedIn](https://www.linkedin.com/in/your-linkedin-username) | 
[Email](mailto:michellesarah.david@gmail.com)
