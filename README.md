# Real-Time Sign Language Detection System

This project implements a real-time sign language recognition system using MediaPipe for hand landmark detection and an LSTM-based deep learning model to classify gestures. It is designed to assist in translating sign language into text using computer vision and sequence modeling.

## Overview

The system captures hand gestures from video input, extracts 543 key landmarks using MediaPipe, and classifies the gestures using an LSTM neural network. The project aims to facilitate accessible communication for individuals relying on sign language.

## Model Architecture

- **MediaPipe**: Used to extract real-time 3D hand landmarks (543 total features per frame).
- **LSTM Network**: Implemented using TensorFlow/Keras to model the temporal dynamics of gestures and classify them.
- **Input**: Live or recorded video stream.
- **Output**: Detected sign language class (text label).

## Features

- Formulated a real-time sign language detection system using **MediaPipe** and **Computer Vision**.
- Extracted 543 hand landmarks from video input to represent spatial hand motion.
- Implemented an LSTM model using **TensorFlow/Keras** to recognize and classify gestures.
- Trained and validated the model on **900 labeled samples** covering multiple signs.
- Achieved **over 80% accuracy** in gesture recognition.

## Technologies Used

- Python
- MediaPipe
- OpenCV
- TensorFlow / Keras
- NumPy
- Scikit-learn
- Matplotlib

## Project Structure

├── dataset/
│ ├── raw_videos/
│ ├── extracted_landmarks/
├── model/
│ ├── lstm_model.py
├── utils/
│ ├── mediapipe_utils.py
│ ├── preprocessing.py
├── train.py
├── predict.py
├── app.py # For real-time inference
├── README.md


## Results

- **Accuracy**: Over 80% on validation data.
- **Robustness**: Recognizes hand gestures across varied lighting and hand positions.
