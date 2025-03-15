Gesture Recognition

A real-time hand gesture recognition system that leverages computer vision, deep learning, and audio processing to detect and classify hand gestures from a live video feed. This project is designed to enhance human-computer interaction and assist with applications such as sign language interpretation and gesture-based control systems.

Table of Contents
Overview
Features
Installation
Usage
Acknowledgment
License

Overview:
This project implements a real-time hand gesture recognition system using a combination of TensorFlow and OpenCV. In addition to image-based gesture recognition, the system includes an audio module that converts recognized gestures into corresponding audio outputs. It aims to create an accessible tool that bridges communication gaps and serves various applications such as assistive technology, smart home controls, and more.

Key aspects include:

Real-time detection: Utilizes a live webcam feed to capture and process gestures on the fly.
Custom Image & Audio Datasets: Allows you to create your own dataset of hand gestures and corresponding audio labels for comprehensive model training.
Model Training: Employs a state-of-the-art object detection model (based on the SSD MobileNet architecture) tailored for gesture recognition.
Practical Deployment: Demonstrates real-time detection with both visual and audio feedback.
Features
Live Video Feed Processing: Uses OpenCV to capture and process video input from a webcam.
Custom Dataset Creation: Easily generate your own image dataset of hand gestures, and link it with an audio dataset that provides corresponding sound outputs.
Model Training & Inference: Train a deep learning model using TensorFlow and deploy it for real-time recognition.
Audio Output Integration: Converts recognized gestures into audio signals using a pre-defined audio label map.
Adaptability: Designed to perform well under various lighting conditions and angles by utilizing a custom-built dataset.
Open Source Inspiration: Inspired by the RealTimeSignLanguageDetectionwithTFJS project by Nick Nochnack.
Installation
Clone the repository:

Clone:
git clone https://github.com/FaiyazShahriar98/Gesture_Recognition.git
Install dependencies: Ensure you have Python 3.x installed. Install the required libraries using pip:

Install Dependencies:
pip install tensorflow opencv-python numpy
Dependencies include TensorFlow 2.x for model training and inference, OpenCV for video processing, NumPy for numerical operations, and additional libraries for audio processing.

Usage
Data Collection (Optional):

Image Dataset: Use the provided image collection script or notebook (e.g., 1. Image Collection.ipynb) to capture images of different hand gestures via your webcam.
Audio Dataset: Collect or create short audio clips corresponding to each hand gesture. Organize these audio files in a folder structure matching your image labels.
Model Training & Detection:
Open the training notebook (e.g., 2_Training_and_Detection_Modified.ipynb) and run the cells to:

Train the gesture recognition model (or load a pre-trained model).
Link the audio output system with the gesture labels using the audio label map.
Launch a real-time demo that shows gesture detection alongside corresponding audio output.
Real-Time Recognition:
When running the demo, perform hand gestures in front of your camera. The system will display the predicted gesture label on the video feed and simultaneously play the associated audio output. Stop the demo by interrupting the notebook execution or closing the video window.

Example:
After installing dependencies, open the notebook and run all cells. The model will train (or load an existing checkpoint), then open a window displaying the live video feed with gesture labels and trigger audio feedback when gestures are recognized.

Acknowledgment
This project was inspired by the open-source project RealTimeSignLanguageDetectionwithTFJS by Nick Nochnack. Their work provided valuable insights and a strong foundation for developing real-time gesture detection and audio integration techniques.

License
This project is released under the MIT License. Feel free to use, modify, and distribute this project in accordance with the terms of the license. See the LICENSE file for details.

