# Hand Gesture Presentation Controller

A Python-based **AI-powered Hand Gesture Presentation Controller** that allows users to control PowerPoint-style presentations using real-time hand gestures through a webcam. The system uses computer vision and hand tracking to navigate slides, draw annotations, undo drawings, clear annotations, and zoom in or out without using a keyboard or mouse.

## 🚀 Project Overview

The Hand Gesture Presentation Controller is designed to make presentations more interactive and convenient by replacing traditional keyboard controls with touchless hand gestures.

Using **OpenCV** and **cvzone HandTrackingModule**, the application detects hand landmarks, identifies finger positions, and performs specific actions based on predefined gestures.

The application displays presentation slides in fullscreen mode while showing a live webcam feed for gesture recognition.

## ✨ Features

- **Gesture-Based Slide Navigation:** Move to the next or previous slide using hand gestures.
- **Gesture Control Toggle:** Enable or disable gesture control using an open-palm gesture.
- **Draw Annotations:** Draw directly on presentation slides using your index finger.
- **Undo Annotations:** Remove the most recent annotation using a three-finger gesture.
- **Clear Annotations:** Clear all drawings from the current slide.
- **Zoom In:** Enlarge presentation slides using a closed-fist gesture.
- **Zoom Out:** Restore the original slide view using a thumb-and-pinky gesture.
- **Real-Time Hand Tracking:** Detect and track hand landmarks through a webcam.
- **Fullscreen Presentation:** Display slides in fullscreen mode.
- **Camera Feed Overlay:** Display a small live webcam preview on the presentation screen.
- **Gesture Cooldown:** Reduce accidental repeated gesture execution.

## 🖐️ Gesture Controls

| Hand Gesture | Action |
|---|---|
| 🖐️ Open Palm | Toggle gesture control ON/OFF |
| 👍 Thumb Up | Previous Slide |
| 🤙 Pinky Up | Next Slide |
| ☝️ Index Finger | Draw annotations |
| ✌️ Index + Middle Finger | Show drawing pointer |
| 🤟 Three Fingers | Undo last annotation |
| 🤏 Thumb + Index Finger | Clear all annotations |
| ✊ Closed Fist | Zoom In |
| 🤙 Thumb + Pinky | Zoom Out |

**Note:** Gesture controls work when gesture control mode is enabled.

## 🛠️ Technologies Used

- **Python** – Core programming language.
- **OpenCV (cv2)** – Image processing, webcam capture, and presentation display.
- **cvzone** – Hand tracking and finger gesture detection.
- **MediaPipe** – Hand landmark detection through cvzone.
- **OS Module** – Accessing and loading presentation images.
- **Time Module** – Managing gesture cooldown intervals.

## 📂 Project Structure

```text
HandGestureController/
│
├── Presentation/
│   ├── slide1.jpg
│   ├── slide2.jpg
│   ├── slide3.jpg
│   └── ...
│
├── HandTracking.py
├── requirements.txt
└── README.md
```

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/KritikaBansode/HandGestureController.git
```

### 2. Navigate to the Project Directory

```bash
cd HandGestureController
```

### 3. Install Dependencies

```bash
pip install opencv-python cvzone mediapipe
```

Alternatively, install dependencies using the requirements file:

```bash
pip install -r requirements.txt
```

### 4. Add Presentation Slides

- Create a folder named `Presentation` in the project directory.
- Add your presentation slides as image files (JPG or PNG).
- Ensure the images are in the correct order.

### 5. Run the Application

```bash
python HandTracking.py
```

### 6. Exit the Application

Press **Q** to close the presentation and release the webcam.

## ⚡ Configuration

The following parameters can be customized in the Python script:

| Parameter | Default Value | Description |
|---|---:|---|
| Screen Width | 1280 | Presentation width |
| Screen Height | 720 | Presentation height |
| Camera Resolution | 640 × 480 | Webcam resolution |
| Detection Confidence | 0.9 | Hand detection confidence |
| Gesture Cooldown | 1 second | Delay between gestures |
| Maximum Zoom | 2.0 | Maximum zoom level |
| Minimum Zoom | 1.0 | Minimum zoom level |

## 🔮 Future Enhancements

- Add support for multiple-hand gesture recognition.
- Integrate voice commands for presentation control.
- Improve gesture recognition accuracy and responsiveness.
- Add support for directly controlling PowerPoint and PDF presentations.
- Implement gesture customization.
- Save annotations for future reference.

## 🎯 Learning Outcomes

Through this project, I gained practical experience in:

- Real-time computer vision applications.
- Hand landmark detection and tracking.
- Finger gesture recognition.
- Image processing using OpenCV.
- Building interactive Python applications.
- Implementing event-based controls using hand gestures.

## 👩‍💻 Author

**Kritika Bansode**

- GitHub: [KritikaBansode](https://github.com/KritikaBansode)
- LinkedIn: [Kritika Bansode](https://www.linkedin.com/in/kritika-bansode-062657281/)

---

⭐ If you find this project interesting, consider giving it a star!
