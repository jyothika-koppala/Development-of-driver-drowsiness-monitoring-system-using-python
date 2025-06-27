# Development-of-driver-drowsiness-monitoring-system-using-python
This Python-based system uses computer vision and facial landmarks to monitor a driver's eye activity in real-time. By calculating the Eye Aspect Ratio (EAR), it detects drowsiness and triggers an alarm if the eyes remain closed beyond a safe limit, helping prevent microsleep-related accidents.
# Driver Drowsiness Monitoring System Using Python

A real-time driver drowsiness detection system using computer vision and Python. This project helps to prevent road accidents by alerting drivers when they show signs of drowsiness.

---

1.Features

- Real-time video stream processing using OpenCV
- Facial landmark detection using dlib
- Calculates Eye Aspect Ratio (EAR) to detect eye closure
- Triggers an alarm if drowsiness is detected
- Simple and efficient Python-based implementation

---

2.Objective

To develop a smart vision-based system that continuously monitors the driver's eye movements and sounds an alert if signs of drowsiness are detected, thereby reducing the risk of accidents.

---

3.Technologies Used

- **Language:** Python 3.x
- **Libraries:**
  - OpenCV
  - dlib
  - imutils
  - scipy
  - playsound or pygame (for alert sound)

---

4.Installation

#1. Clone the Repository

```bash
git clone https://github.com/your-username/driver-drowsiness-monitoring.git
cd driver-drowsiness-monitoring
```
#2.Install Required Packages

```bash
pip install opencv-python dlib imutils scipy playsound
```
5.How It Works
i.The webcam captures video frames.

ii.dlib detects the driver’s face and extracts facial landmarks.

iii.Eye Aspect Ratio (EAR) is calculated for both eyes.

iv.If the EAR is below a set threshold for a number of frames, the system identifies drowsiness.

v.A sound alarm is triggered to alert the driver.

6.Eye Aspect Ratio (EAR)

```bash
EAR = (||p2 - p6|| + ||p3 - p5||) / (2 * ||p1 - p4||)
```
7.Usage

```bash
python drowsiness_detector.py
```

8. File Structure

```bash
driver-drowsiness-monitoring/
├── drowsiness_detector.py
├── shape_predictor_68_face_landmarks.dat
├── alarm.wav
├── README.md
```

9.Future Enhancements

> Integrate with Raspberry Pi and buzzer module

> Add head tilt detection for better accuracy

> Log drowsiness events for analytics

> Use deep learning for better prediction

