# Weapon-Suspicious-Activity-Detection-OPENCV

This project implements a security monitoring system using computer vision techniques to detect and respond to potential security threats. The system combines face emotion recognition and weapon detection to enhance security in a given environment.

## Features

- **Face Emotion Recognition:** The system utilizes a pre-trained deep learning model to recognize emotions on human faces captured by a camera feed. It can detect emotions such as anger, fear, happiness, sadness, surprise, and more.

- **Weapon Detection:** The system employs YOLO (You Only Look Once) object detection to identify weapons within the camera feed. When a weapon is detected, it raises an alarm.

- **Suspicious Activity Detection:** The system can identify suspicious activities based on detected emotions and weapon presence. It raises a flag for suspicious activity if certain conditions are met.

## Prerequisites

Before running the script, make sure you have the following prerequisites:

- Python 3.x
- OpenCV (cv2) library
- NumPy library
- TensorFlow library (for the emotion recognition model)
- A trained emotion recognition model (in the example, "FacialExpressionModel.h5" is used)
- YOLO weights and configuration files for weapon detection

You can download the trained emotion recognition model from this [Google Drive link](https://drive.google.com/drive/folders/1DtSixBhCt3Ac2IxRnLDiaWtLzimh7MGi?usp=sharing).

You can obtain the YOLO configuration files and weights from this [Google Drive link](https://drive.google.com/drive/folders/1DtSixBhCt3Ac2IxRnLDiaWtLzimh7MGi?usp=sharing).

## Installation

Install the necessary Python libraries using pip:
```
pip install opencv-python numpy tensorflow
```

## Usage
  - Update Paths: Open the security_monitoring_system.py file in a text editor and update the paths to the emotion recognition model, YOLO weights, and configuration files.

  - Run the Script: Execute the Python script security_monitoring_system.py to start the security monitoring system:
    ```
    python security_monitoring_system.py
    ```
  - Camera Feed: The system will open a camera feed and start detecting emotions, weapons, and suspicious activities in real-time.

## Script Explanation
The script utilizes Haar Cascade classifier for face detection and YOLO for weapon detection.
Emotion recognition is performed using a pre-trained deep learning model loaded with TensorFlow.
The script uses multi-threading to process face emotion recognition and weapon detection simultaneously, improving performance.
Detected emotions, weapon presence, and suspicious activity flags are displayed in real-time on the camera feed.

## Contributing
Contributions to the project are welcome! If you have any ideas for improvement, suggestions, or bug fixes, feel free to open an issue or create a pull request.

## License
This project is licensed under the MIT License. Feel free to use and modify it according to your needs.


