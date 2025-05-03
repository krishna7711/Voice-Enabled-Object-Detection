#Voice-Enabled Object Detection for the Visually Impaired using CNN
Overview
This project implements a voice-assisted object detection system designed to aid visually impaired individuals by identifying objects in real-time using a camera and conveying the results through audio output. The system utilizes a Convolutional Neural Network (CNN) and deep learning techniques integrated with voice-based technology to provide an accessible and intelligent solution for navigation and object recognition.

Features
Real-time object detection using YOLOv3 model.

Voice-based interface for initiating detection.

Audio feedback announcing detected objects.

Raspberry Pi integration for portability.

Uses OpenCV, TensorFlow, and Pyttsx3 libraries.

Technologies Used
Programming Language: Python

Deep Learning Framework: TensorFlow

Object Detection Model: YOLOv3 (You Only Look Once)

Libraries: OpenCV, Pyttsx3, SpeechRecognition

Hardware: Raspberry Pi, USB Camera

System Architecture
Voice Input: Captures user's voice command using microphone.

Speech Recognition: Processes the voice input to trigger detection.

Object Detection: Detects objects using YOLOv3 via OpenCV.

Text-to-Speech: Announces the detected objects using Pyttsx3.

Output: Audible feedback of identified objects.

Installation
Clone this repository:

bash
Copy
Edit
git clone https://github.com/your-username/voice-object-detection.git
cd voice-object-detection
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Set up YOLOv3 weights and configuration files (place in yolo-coco directory):

yolov3.cfg

yolov3.weights

coco.names

Run the application:

bash
Copy
Edit
python main.py
Usage
Speak the trigger word (e.g., "detect") to initiate object detection.

The system captures video frames and processes them in real-time.

Detected objects are spoken aloud via a speaker or headphones.

Project Structure
css
Copy
Edit
voice-object-detection/
├── yolo-coco/
│   ├── yolov3.cfg
│   ├── yolov3.weights
│   └── coco.names
├── main.py
├── speech_module.py
├── detection_module.py
├── requirements.txt
└── README.md
Contributors
Bolla Leela Krihsna Mohan

License
This project is licensed under the MIT License.
