# Hand Gesture Volume Control

![License](https://img.shields.io/badge/License-MIT-blue.svg)
![Status](https://img.shields.io/badge/status-active-brightgreen)
![Built With](https://img.shields.io/badge/Tech-OpenCV%20%7C%20MediaPipe%20%7C%20PyCaw-blue)

Control your system volume using simple **hand gestures** via webcam. This real-time computer vision project uses **OpenCV + MediaPipe** for hand tracking and **PyCaw** for system-level audio control on Windows.

---

## ✨ Features

- 🖐️ Real-time hand detection using webcam
- 🔊 Adjust system volume by changing distance between **thumb and index finger**
- 🔒 Safety confirmation using pinky finger (only adjusts when pinky is down)
- 📊 On-screen volume bar and FPS counter
- 🧠 Works entirely hands-free with visual feedback

---

## 🛠️ Tech Stack

| Component        | Technology             |
|------------------|-------------------------|
| Hand Tracking    | MediaPipe               |
| Image Processing | OpenCV, NumPy           |
| Volume Control   | PyCaw, comtypes (Windows) |
| Language         | Python 3.8+             |

---

## 📁 Project Structure

```
hand-gesture-volume-control/
├── volumeControl.py           # Main script with hand detection & volume logic
├── HandTrackingModule.py      # Reusable hand tracking helper class
├── .gitignore                 # Python cache/files to ignore
├── LICENSE                    # MIT License
└── README.md                  # Project documentation
```

---

## 📦 Installation

### ✅ Prerequisites

- Python 3.8 or higher
- A webcam (built-in or external)
- Windows OS (PyCaw works only on Windows)

### 🧪 Install Dependencies

```bash
pip install opencv-python mediapipe numpy pycaw comtypes
```

---

## 🚀 How to Run

1. Clone or download the repository
2. Ensure your webcam is connected
3. Run the script:

```bash
python volumeControl.py
```

> ℹ️ If webcam doesn't open, try changing this line in `volumeControl.py`:

```python
cap = cv2.VideoCapture(0)  ➝  cap = cv2.VideoCapture(1)
```

---

## 🔍 How It Works

- The webcam detects your hand using MediaPipe.
- Distance between **thumb tip and index tip** is calculated in real time.
- When **pinky is lowered**, the measured distance is mapped to system volume levels.
- A **volume bar**, **percentage**, and **FPS** are rendered on the screen.

---

## 📸 Demo (Optional)

> You can add demo images/GIFs in a `docs/` folder here.

---

## 📌 To-Do / Enhancements

- [ ] Add audio feedback on volume change
- [ ] Cross-platform volume control (Linux/Mac)
- [ ] GUI with volume slider
- [ ] Hand gesture toggle (enable/disable volume mode)

---

## 🙏 Acknowledgments

- [MediaPipe](https://mediapipe.dev/) for real-time hand tracking  
- [PyCaw](https://github.com/AndreMiras/pycaw) for system volume control  
- Inspired by projects from [ComputerVision.Zone](https://www.computervision.zone/)

---

## 👤 Author

**Hridey Dalal**  
📧 [hrideydalal1@gmail.com](mailto:hrideydalal1@gmail.com)  
🔗 [LinkedIn](https://www.linkedin.com/in/hridey-/)

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
