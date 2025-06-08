# Auto Selfie Capture for Smiling Faces using Python

This project captures a selfie automatically when a person smiles, using a webcam feed and facial landmarks detection powered by MediaPipe. When a smile is detected (based on facial landmark distance), a snapshot is saved and a notification sound is played.

# Features

Real-time face tracking using MediaPipe's FaceMesh

Detects a smiling gesture based on the distance between specific facial landmarks

Captures and saves a selfie when a smile is detected

Plays a sound notification on successful capture

No button press required — it's fully automatic!

# How It Works

The script uses MediaPipe FaceMesh to detect facial landmarks.

Landmarks with ID 43 and 287 are tracked — corners of the mouth.

If the Euclidean distance between them exceeds a smile threshold (99 pixels), it assumes a smile.

When a smile is detected:

A snapshot is saved as selfie.png

A sound is played using the winsound module

# Libraries
pip install opencv-python mediapipe pyautogui

# How to run ?

1. Place a smile detection sound (sound.wav) in the correct path (adjust if needed).

2. Run the Python script: python auto_selfie_smile.py
3. Look at the webcam and smile 😊

4. When a smile is detected:

   It saves selfie.png in the current directory.

   Plays the configured .wav sound.

5. Press ESC to exit.

# Acknowledgments

1. MediaPipe by Google for face mesh tracking

2. OpenCV for camera input and image handling

3. winsound for sound alerts (Windows only)


