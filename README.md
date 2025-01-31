# Disaster Management Drone for Human Detection

## Overview
This project implements a **machine learning-based human detection system** on a drone to assist in **disaster response and search-and-rescue operations**. By deploying a **YOLO-V3 deep learning model** on **NVIDIA Jetson TX2**, the system enables real-time human detection in aerial imagery, aiding emergency teams in locating survivors efficiently.

## Features
- **Machine Learning Deployment**: Integrated **YOLO-V3** for real-time human detection using aerial footage.
- **Model Optimization**: Fine-tuned hyperparameters and modified network architecture for enhanced accuracy.
- **Improved Small-Scale Detection**: Recalculated anchor boxes using **k-means clustering** to improve detection of distant or small human figures.
- **High Precision**: Achieved a **70% precision rate**, enhancing the reliability of human detection in disaster zones.

## Technologies Used
- **Deep Learning**: YOLO-V3 (You Only Look Once) for object detection.
- **Hardware**: NVIDIA Jetson TX2 for edge AI processing.
- **Programming Languages**: Python.
- **Frameworks & Libraries**: OpenCV, TensorFlow/PyTorch, CUDA for accelerated computing.

## Installation & Usage
1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/disaster-management-drone.git
   cd disaster-management-drone
   ```

2. **Set Up the Environment**
   Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. **Deploy the Model on Jetson TX2**
   - Load the trained YOLO-V3 model.
   - Run inference on real-time drone footage.
   ```bash
   python detect.py --model yolov3.weights --source drone_feed.mp4
   ```

## Results & Impact
This system significantly enhances disaster response capabilities by enabling drones to autonomously locate survivors in hazardous environments, reducing search time and increasing efficiency in rescue missions.

## Future Improvements
- Upgrade to later YOLO versions for better accuracy and performance.
- Segment the feed into dry lands and water bodies
- Implement **thermal imaging** for night-time search and rescue.
- Optimize **real-time processing** using TensorRT.

---
### Acknowledgments
Special thanks to KLE Technological University, Hubli for supporting this project.
