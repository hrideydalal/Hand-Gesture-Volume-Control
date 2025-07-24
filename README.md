# Hand Gesture Volume Control

This project enables users to control their computer's volume using hand gestures detected via a webcam. It uses OpenCV and MediaPipe for real-time hand tracking, and PyCaw for system volume control (Windows only).

## Features

- Real-time hand detection using webcam
- Volume control by measuring distance between thumb and index finger
- Volume bar and FPS counter overlay on screen
- Visual feedback when volume is adjusted
- Works with one hand, includes pinky finger check for confirmation

## Technologies Used

- Python
- OpenCV
- MediaPipe
- NumPy
- PyCaw
- comtypes (for COM interfacing)

## File Structure

```
hand-gesture-volume-control/
├── volumeControl.py           # Main script for gesture-based volume control
├── HandTrackingModule.py      # Helper module for hand tracking
├── README.md                  # Project documentation
├── .gitignore
└── LICENSE
```

## How to Run

1. Make sure Python is installed and a webcam is available.
2. Install required packages:

```bash
pip install opencv-python mediapipe numpy pycaw comtypes
```

3. Run the script:

```bash
python volumeControl.py
```

Note: If the webcam does not open, try changing `cv2.VideoCapture(0)` to `cv2.VideoCapture(1)` in the code.

## Acknowledgments

- MediaPipe Hand Tracking: https://mediapipe.dev/
- PyCaw (Python Core Audio Windows Library): https://github.com/AndreMiras/pycaw
- Based on a learning project from ComputerVision.Zone

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.

## Author

Hridey Dalal  
B.Tech Computer Science, Sharda University  
LinkedIn: https://www.linkedin.com/in/hridey-
