

## Project Overview
This project implements a **real-time driver monitoring system** using **computer vision techniques** to detect driver fatigue and distraction.  
The system leverages **facial landmark detection, eye-blink analysis, and yawning detection** to monitor the driver’s attentiveness and provide early warnings, thereby reducing the risk of accidents.

##  Features
- **Blink Detection** – Monitors eye closure frequency to detect drowsiness.
- **Yawn Detection** – Identifies yawning patterns using facial landmarks.
- **Head Pose Estimation** – Tracks head movement to detect distraction.
- **Hands-Free Detection** – Ensures driver maintains hands on the wheel.
- **Real-Time Processing** – Uses live video feed for instant feedback.
- **Graphical User Interface (GUI)** – Provides an interactive interface for monitoring.

## Tech Stack
- **Language:** Python
- **Libraries/Frameworks:** OpenCV, Dlib, PyQt5
- **Model/Data:** `shape_predictor_68_face_landmarks.dat` for facial landmark detection

## Project Structure
```

Driver-Monitoring-System/
│── BlinkDetection.py          # Eye blink detection module
│── YawnDetection.py           # Yawn detection module
│── headEst.py                 # Head pose estimation
│── HandsFreeDetection.py      # Hands-free monitoring
│── main.py                    # Main driver code
│── LoginUI.py / LoginUI.ui    # GUI files
│── dataPack.py                # Data handling
│── res\_rc.py / res\_rc.qrc     # Resource files
│── shape\_predictor\_68\_face\_landmarks.dat # Landmark model
│── requirements.txt           # Dependencies
│── README.md                  # Documentation

````

##  Installation & Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Driver-Monitoring-System.git
   cd Driver-Monitoring-System
````

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the application:

   ```bash
   python main.py
   ```

## How It Works

* The system captures **real-time video feed**.
* Detects **facial landmarks** using Dlib’s pretrained model.
* Analyzes eye aspect ratio (EAR) and mouth aspect ratio (MAR) for blink/yawn detection.
* Tracks head movement for distraction monitoring.
* Provides alerts if the driver shows signs of **fatigue** or **inattention**.

##  Use Cases

* Road safety enhancement
* Automotive industry integration
* Research in **human-computer interaction**
* Smart vehicles and self-driving systems

##  Sample UI

*(Include screenshots here if available, e.g. `background1.png`, `window.ui`)*

##  License

This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.


