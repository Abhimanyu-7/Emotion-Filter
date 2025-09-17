# Emotion-Based Real-Time Video Filters
An interactive Python application that uses your webcam to detect facial emotions and applies corresponding real-time visual filters to the video stream.

## Description
This project leverages the power of computer vision to create an engaging and interactive experience. The application captures video from a webcam, detects faces, and analyzes them to determine the user's emotion. Based on the detected emotion, a dynamic and thematic filter is overlaid on the video, creating a visual representation of the user's mood.

> For example, a happy expression might trigger a `sunshine effect` , while a sad expression could make it `rain on screen`. It's a fun demonstration of real-time image processing and facial emotion recognition.

## Demo

![ezgif-1ee4b46d6fe5a9 (1)](https://github.com/user-attachments/assets/5f48cd30-5867-4b0a-a1db-34164e90ba67)



## Features
Real-Time Face Detection: Utilizes OpenCV's Haar Cascades to detect faces in the video feed.

#### Multi-Emotion Recognition: 
1. Employs the fer library to recognize several emotions, including:
  - Happy 😊
  - Sad 😢
  - Surprise 😮
  - Angry 😠
2. Dynamic Visual Filters:
    > Applies unique, animated filters corresponding to the detected emotion:
      - Happy: A warm sunshine overlay with a sun graphic in the corner.
      - Sad: A blue-tinted screen with a falling rain effect.
      - Surprise: A cartoon cloud with a random lightning effect appears over the user's head.
      - Angry: A red tint is applied to the screen with animated steam/fumes.

3. Emotion Smoothing: Averages the last few emotion detections to provide a more stable filter experience and prevent rapid flickering.

### Tech Stack
- Python
- OpenCV (opencv-python):
         > For video capture, face detection, and image manipulation.
- FER (fer): For facial emotion recognition, using TensorFlow as its backend.
- NumPy: For efficient array manipulation and numerical operations.


### Installation
To get this project running on your local machine, follow these steps.

Clone the repository:

Create a virtual environment (Recommended):

Install the required dependencies:
(You should create a requirements.txt file with the libraries: opencv-python, fer, tensorflow, numpy)

Ensure you have the image assets:
Make sure the image files (sun.png, cloud.png, fumes.png) are present in the same directory as the Python script.
