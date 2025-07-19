# Robotic Arm for Automated Waste Segregation

This is a capstone project aimed at automating the waste segregation process using a robotic arm powered by computer vision. The system identifies and classifies waste items into five categories — **plastic, paper, metal, cardboard, and glass** — using a YOLOv8 object detection model.

## 🚀 Project Status

✅ YOLOv8 model trained  
✅ `.pt` file generated  
🔄 Hardware integration and deployment in progress  
🔄 Real-time detection on Raspberry Pi + Pi Camera (planned)  
🔄 Microcontroller and actuator integration (planned)

---

## 🧠 Technologies Used

- Python  
- YOLOv8 (Ultralytics)  
- Roboflow (for dataset annotation)  
- OpenCV (planned for integration)  
- Raspberry Pi (for edge deployment)  
- Pi Camera  
- Microcontroller + DC Motors + Sensors (Ultrasonic, IR, Gyroscope, GPS)

---

## 📂 Dataset

The dataset was collected from both online sources and live campus environments. It was annotated using **Roboflow**, formatted for YOLOv8 training. The classes include:

- Plastic  
- Paper  
- Metal  
- Cardboard  
- Glass

---

## 🧪 Model Training

We used the Ultralytics YOLOv8 framework for training. The dataset was split into training, validation, and testing sets. The final model `.pt` file is ready for deployment on edge hardware.

```bash
# Example command used for training
yolo task=detect mode=train model=yolov8n.pt data=capstone.yaml epochs=50 imgsz=640
