# EyeMaster_FinaleYear_Project

## Virtual Mouse Control using Hand and Eye Gestures
This project implements a virtual mouse system that allows users to control their mouse cursor using hand and eye movements. The system utilizes computer vision techniques, leveraging OpenCV and Mediapipe for real-time hand and face landmark detection. The project is divided into two main parts: hand-controlled mouse and eye-controlled mouse.

## Features
### Hand-Controlled Mouse
Hand Landmark Detection: Uses Mediapipe's hand tracking module to detect and track hand landmarks.
Cursor Movement: The index finger's tip is mapped to the screen coordinates to control the mouse cursor.
Click Simulation: The distance between the thumb and middle finger is calculated to simulate a mouse click. If the fingers come close enough, a click is triggered.

### Eye-Controlled Mouse
Face Mesh Detection: Uses Mediapipe's face mesh module to detect landmarks around the eyes.
Cursor Control: Eye movements are tracked and mapped to screen coordinates, allowing the cursor to follow the user's gaze.
Blink Detection: A click is simulated when the user blinks, detected by the relative positions of specific eye landmarks.

# Prerequisites
Python
OpenCV
Mediapipe
PyAutoGUI

# You can install the required packages using pip:
pip install opencv-python mediapipe pyautogui
How to Run
Clone the repository: git clone https://github.com/yourusername/virtual-mouse-control.git
cd virtual-mouse-control

# Run the script:python hand_controlled_mouse.py
For hand-controlled mouse
python eye_controlled_mouse.py 
For eye-controlled mouse

Memory updated
Here’s a draft for your GitHub README:

Virtual Mouse Control using Hand and Eye Gestures
This project implements a virtual mouse system that allows users to control their mouse cursor using hand and eye movements. The system utilizes computer vision techniques, leveraging OpenCV and Mediapipe for real-time hand and face landmark detection. The project is divided into two main parts: hand-controlled mouse and eye-controlled mouse.

Features
Hand-Controlled Mouse
Hand Landmark Detection: Uses Mediapipe's hand tracking module to detect and track hand landmarks.
Cursor Movement: The index finger's tip is mapped to the screen coordinates to control the mouse cursor.
Click Simulation: The distance between the thumb and middle finger is calculated to simulate a mouse click. If the fingers come close enough, a click is triggered.
Eye-Controlled Mouse
Face Mesh Detection: Uses Mediapipe's face mesh module to detect landmarks around the eyes.
Cursor Control: Eye movements are tracked and mapped to screen coordinates, allowing the cursor to follow the user's gaze.
Blink Detection: A click is simulated when the user blinks, detected by the relative positions of specific eye landmarks.
Prerequisites
Python 3.x
OpenCV
Mediapipe
PyAutoGUI
Tkinter (for screen resolution)
You can install the required packages using pip:

bash
Copy code
pip install opencv-python mediapipe pyautogui
How to Run
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/virtual-mouse-control.git
cd virtual-mouse-control
Run the script:

bash
Copy code
python hand_controlled_mouse.py  # For hand-controlled mouse
python eye_controlled_mouse.py   # For eye-controlled mouse
Press 'q' to quit the application at any time.

# How It Works
### Hand-Controlled Mouse
The script captures video from your webcam and processes each frame to detect hand landmarks.
The index finger's tip coordinates are converted to screen coordinates, allowing you to move the mouse pointer.
The distance between the thumb and middle finger controls the click action.
### Eye-Controlled Mouse
The script captures video and detects facial landmarks focusing on the eyes.
Specific landmarks around the eyes are used to track eye movements, which are then mapped to screen coordinates.
A click action is simulated based on the blink detection using the relative positions of eye landmarks.
