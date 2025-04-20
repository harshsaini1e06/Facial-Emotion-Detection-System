
# Project Title

A brief description of what this project does and who it's for

# Facial Emotion Detection System

A deep learning project for detecting human facial emotions in real-time using a webcam. This system uses a Convolutional Neural Network (CNN) trained on facial emotion images and deployed using OpenCV for live video capture and emotion classification.

## 🧠 Features

- Real-time facial emotion recognition using webcam input
- Detects 7 emotions: Angry, Disgust, Fear, Happy, Neutral, Sad, Surprise
- Uses Haar Cascade for face detection
- Trained using Keras/TensorFlow with grayscale 48x48 images

## 📁 Project other requirenment

-Ensure that your system has a working webcam and Python 3.6+ installed.

🧪 Model Training

  ->Open trainmodel.ipynb and run the cells to:

  - Load and preprocess the dataset (e.g., FER2013 or custom)
  - Train a CNN on grayscale facial images (48x48)
  - Save the model architecture (facialemotionmodel.json)
  - Save the trained weights (facialemotionmodel.h5)

🎥 Real-Time Emotion Detection

  ->To run the real-time emotion detection:
  - Ensure facialemotionmodel.json and facialemotionmodel.h5 are in the same directory.

  ->Run the detection script:
  - python realtimedetection.py

A webcam window will pop up showing detected faces with predicted emotion labels.

🎯 Emotion Labels

  ->The model classifies faces into the following emotions:

  0: Angry
  1: Disgust
  2: Fear
  3: Happy
  4: Neutral
  5: Sad
  6: Surprise

📌 Notes

  - Make sure lighting conditions are good for accurate detection.
  - Resize input images to 48x48 grayscale during both training and inference.
  - The model uses Haar Cascades which are fast but may miss faces in extreme angles or occlusions.

🤝 Contributing

Contributions, improvements, and suggestions are welcome! Please fork the repo and open a pull request.


## 🛠️ Requirements

Install dependencies using pip:

```bash
pip install opencv-python tensorflow keras numpy
