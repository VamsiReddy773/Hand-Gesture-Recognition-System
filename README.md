# Hand Gesture Recognition System
This project is a real-time hand gesture recognition system that uses MediaPipe for hand tracking and pyautogui for gesture-based control. The system detects hand gestures and maps them to specific keyboard actions, enabling intuitive human-computer interaction.

# Features

Real-Time Hand Tracking: Uses MediaPipe to detect and track 21 hand landmarks in real-time.
Gesture Classification: Classifies gestures based on the number of raised fingers.
Gesture Control: Maps specific gestures to keyboard actions (e.g., pressing "right", "left", "up", "down", or "space").
Visual Feedback: Displays hand landmarks and connections on the screen for real-time feedback.

# Requirements

To run this project, you need the following Python libraries:

OpenCV: For video capture and image processing.
MediaPipe: For hand tracking and landmark detection.
pyautogui: For simulating keyboard actions based on gestures.
You can install the required libraries using the following command:

bash
Copy
pip install opencv-python mediapipe pyautogui
Project Structure

The project is organized into the following files:

hand_tracking.py:
Initializes the MediaPipe Hands module for hand tracking.
Captures the webcam feed for real-time video processing.
gesture_classification.py:
Contains the logic for counting the number of raised fingers based on hand landmarks.
gesture_control.py:
Maps specific gestures to keyboard actions using pyautogui.
main.py:
Integrates all modules for real-time gesture recognition and control.
How to Run the Project

Clone the repository:
bash
Copy
git clone https://github.com/your-username/hand-gesture-recognition.git
cd hand-gesture-recognition
Install the required dependencies:
bash
Copy
pip install -r requirements.txt
Run the main.py file:
bash
Copy
python main.py
Use the following gestures to control the system:
1 Finger: Press "right"
2 Fingers: Press "left"
3 Fingers: Press "up"
4 Fingers: Press "down"
5 Fingers: Press "space"
Press the Esc key to exit the program.
Code Overview

1. Hand Tracking (hand_tracking.py)

Initializes the MediaPipe Hands module for hand tracking.
Captures the webcam feed for real-time video processing.
2. Gesture Classification (gesture_classification.py)

Counts the number of raised fingers based on the positions of hand landmarks.
3. Gesture Control (gesture_control.py)

Maps specific gestures to keyboard actions using pyautogui.
4. Main Execution (main.py)

Integrates all modules for real-time gesture recognition and control.
Example Usage

python
Copy
# Load data
data1 = load_data("Samsung_Galaxy_S23_FE.csv")
data2 = load_data("OnePlus_11R_5g.csv")
data3 = load_data("Oneplus_Nord_3_5g.csv")

# Preprocess data
data1 = preprocess_data(data1)
data2 = preprocess_data(data2)
data3 = preprocess_data(data3)

# Clean text data
data1['cleaned_text'] = data1['text_column'].apply(text_preprocessing)
Future Enhancements

Model Training: Integrate a machine learning model (e.g., LSTM) for more advanced gesture recognition.
Multi-Gesture Support: Extend the system to recognize more complex gestures.
Edge Deployment: Optimize the code for deployment on edge devices like smartphones or Raspberry Pi.
User Interface: Add a graphical user interface (GUI) for better user interaction.
Contributing

Contributions are welcome! If you'd like to contribute to this project, please follow these steps:

Fork the repository.
Create a new branch for your feature or bug fix.
Commit your changes and push them to your branch.
Submit a pull request.
