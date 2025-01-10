# Hand Gesture Recognition System

This project implements a Hand Gesture Recognition System using Python, OpenCV, and Mediapipe. The system detects hand gestures via a webcam and performs specific actions such as simulating keyboard key presses based on the number of fingers detected.

## How to Run

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/gesture-control-system.git
    cd gesture-control-system
    ```

2. Run the script:
    ```bash
    python gesture_control.py
    ```

3. Ensure your webcam is properly connected and active.

4. Use the following gestures to control the system:
    - **1 Finger**: Press the "Right Arrow" key.
    - **2 Fingers**: Press the "Left Arrow" key.
    - **3 Fingers**: Press the "Up Arrow" key.
    - **4 Fingers**: Press the "Down Arrow" key.
    - **5 Fingers**: Press the "Space" key.

5. Press the `Esc` key to exit the application.

## Project Workflow

1. **Capture Webcam Input**: Uses OpenCV to capture and display the video feed.
2. **Hand Detection**: Mediapipe's hand tracking module identifies and tracks hand landmarks.
3. **Finger Counting**: A custom algorithm calculates the number of raised fingers.
4. **Key Simulation**: PyAutoGUI simulates the corresponding keyboard key press.

## Demo

*(Replace this placeholder with an actual demo GIF showing the system in action.)*

![Demo GIF](https://via.placeholder.com/800x400?text=Demo+GIF)

## Future Enhancements

- Add support for more gestures.
- Implement gesture customization.
- Optimize finger detection algorithm for better accuracy.
- Enable multi-hand gesture recognition.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Mediapipe](https://mediapipe.dev) by Google for hand tracking.
- [OpenCV](https://opencv.org/) for video capture and processing.
- [PyAutoGUI](https://pyautogui.readthedocs.io/) for simulating keyboard actions.

## Contributing

Feel free to fork this repository and submit pull requests for improvements or new features!

## Author

**Vamsi Krishna Reddy**  
Passionate about integrating AI and technology into daily life.

---

### Happy Coding!
