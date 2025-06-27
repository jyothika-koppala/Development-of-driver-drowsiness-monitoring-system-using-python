# Development-of-driver-drowsiness-monitoring-system-using-python
This Python-based system uses computer vision and facial landmarks to monitor a driver's eye activity in real-time. By calculating the Eye Aspect Ratio (EAR), it detects drowsiness and triggers an alarm if the eyes remain closed beyond a safe limit, helping prevent microsleep-related accidents.
# 1.Driver Drowsiness Monitoring System Using Python

A real-time driver drowsiness detection system using computer vision and Python. This project helps to prevent road accidents by alerting drivers when they show signs of drowsiness.

---

##2.Features

- Real-time video stream processing using OpenCV
- Facial landmark detection using dlib
- Calculates Eye Aspect Ratio (EAR) to detect eye closure
- Triggers an alarm if drowsiness is detected
- Simple and efficient Python-based implementation

---

##3.Objective

To develop a smart vision-based system that continuously monitors the driver's eye movements and sounds an alert if signs of drowsiness are detected, thereby reducing the risk of accidents.

---

##4.Technologies Used

- **Language:** Python 3.x
- **Libraries:**
  - OpenCV
  - dlib
  - imutils
  - scipy
  - playsound or pygame (for alert sound)

---

##5.Installation

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/driver-drowsiness-monitoring.git
cd driver-drowsiness-monitoring
### 2.Install required packages
pip install opencv-python dlib imutils scipy playsound

 How It Works
>The webcam captures video frames.

>dlib detects the driver’s face and extracts facial landmarks.

>Eye Aspect Ratio (EAR) is calculated for both eyes.

>If the EAR is below a set threshold for a number of frames, the system identifies drowsiness.

>A sound alarm is triggered to alert the driver.

##6.Eye Aspect Ratio (EAR)
EAR = (||p2 - p6|| + ||p3 - p5||) / (2 * ||p1 - p4||)

##7.Usage
python drowsiness_detector.py
