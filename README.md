# Real-Time Emotion Detection using OpenCV and DeepFace

## Overview

This project implements a real-time emotion detection system using computer vision techniques and deep learning. It captures live video from a webcam, detects human faces in the frames, and classifies the emotions displayed on the faces using the `DeepFace` library. The detected emotions are then displayed on the video feed in real-time.

## Features

- Real-time video capture and processing using OpenCV.
- Face detection using a Haar Cascade classifier.
- Emotion analysis and classification using `DeepFace`.
- Display detected emotions on faces in the live video feed.
- Simple to use with minimal setup.

## Technologies Used

- **Python**: The programming language used to build the application.
- **OpenCV**: For video capture and face detection.
- **DeepFace**: For emotion analysis using deep learning models.
- **Haar Cascade**: Used for face detection.

## Prerequisites

- Python 3.x
- Webcam or camera for real-time video capture

## Installation

1. **Clone the Repository**

    ```bash
    git clone https://github.com/your-username/emotion-detection.git
    cd emotion-detection
    ```

2. **Create a Virtual Environment (Optional)**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

3. **Install Dependencies**

    Install the required Python packages using `pip`:

    ```bash
    pip install opencv-python deepface
    ```

4. **Verify Installation**

    - Make sure the `haarcascade_frontalface_alt.xml` file is present in the OpenCV data directory. This is used for face detection.

## Usage

1. **Run the Emotion Detection Script**

    Execute the main Python script:

    ```bash
    python main.py
    ```

2. **Operating the Application**

    - A window will open, displaying the live video feed from your webcam.
    - Detected faces will be highlighted with rectangles, and the dominant emotion will be displayed above each face.
    - Press the **'q'** key to stop the video stream and close the application.

## Code Breakdown

- **Step 1:** Import libraries (`cv2` for OpenCV and `DeepFace` for emotion analysis).
- **Step 2:** Load the Haar Cascade XML file for face detection.
- **Step 3:** Open a video stream using the default webcam.
- **Step 4:** Process each frame, detect faces, and use `DeepFace` to analyze emotions.
- **Step 5:** Display the detected faces and emotions on the live video feed.
- **Step 6:** Exit the video stream when the 'q' key is pressed.

## Example Output

![Sample Output](path/to/sample_output.png)

This is what the real-time emotion detection looks like, with rectangles drawn around faces and emotion labels displayed on the frame.

## Project Structure

```plaintext
emotion-detection/
│
├── haarcascade/                   # Directory for Haar Cascade XML file
│   └── haarcascade_frontalface_alt.xml
│
├── main.py                        # Main script for real-time emotion detection
│
├── README.md                      # This file
│
└── requirements.txt               # List of required Python packages
