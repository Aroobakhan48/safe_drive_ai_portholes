# Road Pothole Detection Model

This project is a **Deep Learning based Object Detection model** that detects **potholes on roads** from images and videos.  
The model is trained using **YOLOv8** with a custom dataset labeled in **COCO format**.

---

##  Features
- Detects potholes in real-time using webcam or video input.
- Trained on a custom dataset with labeled potholes.
- Supports both **image and live camera detection**.
- Can be integrated into **road safety applications**.

---

## Project Structure

├── dataset/ # Training dataset (COCO format)
├── runs/ # Training results and checkpoints
├── best.pt # Trained YOLOv8 model weights
├── detect_with_cam.py # Script for real-time detection via webcam
├── requirements.txt # Dependencies
└── README.md # Project documentation


---

##  Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/YourUsername/Road-Pothole-Detection.git
   cd Road-Pothole-Detection

Create virtual environment (optional but recommended):
python -m venv venv
source venv/bin/activate   # On Linux/Mac
venv\Scripts\activate      # On Windows

Install dependencies:
pip install -r requirements.txt

Training

To train the model on your dataset:
yolo task=detect mode=train model=yolov8n.pt data=data.yaml epochs=50 imgsz=640
Inference
Detect objects in an image:
yolo task=detect mode=predict model=best.pt source="test.jpg"

Real-time webcam detection:
python detect_with_cam.py
Results

Model: YOLOv8

Epochs: 50

mAP50: 79%

mAP50-95: 90%

Future Work

Extend dataset with more diverse pothole images.

Deploy as a mobile application.

Integrate with IoT sensors for smart road monitoring.
Author

AROOBA KHAN
HCCDA-AI , UET LAHORE
BS Mathematics, Punjab University

License
This project is licensed under the MIT License.
 
 Project ka **safe_drive_ai_potholes**  
 
  



