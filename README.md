Project Overview and Results: Transport Mode Detection

Project Objectives:

This project aims to develop a real-time detection system capable of identifying a wide range of transport modes, including:

Cars
![alt text](image.png)
Buses
Motorcycles
Boats
Trains
Airplanes
Bicycles
The model utilizes the YOLOv4 (You Only Look Once) algorithm, known for its high performance, speed, and efficiency in object detection in complex environments.

Motivation and Context:

Transport mode detection plays a crucial role in various fields:

Smart urban traffic management to monitor and analyze vehicle flows.
Public safety, such as detecting suspicious vehicles or monitoring critical infrastructures.
Maritime, air, and rail transport to improve logistics and resource management.
Development of autonomous vehicles, providing a reliable detection foundation.
With the growing need for automation and real-time video analysis, this project addresses significant technological and societal challenges.

Results Obtained:

Extended Multi-Class Detection: The model is capable of detecting various types of transport modes while recognizing other objects present in the environment, such as people, traffic lights, stop signs, etc.

Accuracy and Reliability: The system achieves high accuracy (mAP - Mean Average Precision) in detecting vehicles, including buses, motorcycles, and trains. Confidence thresholds are optimized to minimize false positives while capturing relevant objects.

Real-Time Performance: Thanks to the efficiency of YOLOv4 and optimization of the implementation via OpenCV, the model runs smoothly on live video streams.

Examples of Use:

Simultaneous detection of cars and buses in urban areas.
Identification of boats and airplanes in aerial or maritime images.
Project Importance:

Societal Impact: This project can contribute to innovative solutions for transportation management and road safety by providing automated, real-time tools.

Flexibility and Scalability: The system can easily be adapted to detect other objects or classes based on specific needs.

High-Performance Technology: By using a proven model like YOLOv4 and accessible frameworks like OpenCV, this project offers a powerful and adaptable solution for various applications in object detection.

This system demonstrates the effectiveness of modern deep learning algorithms applied to real-world and complex problems, with potential applications in key sectors such as transportation, logistics, and smart surveillance.

Source Code:
The source code for the transport mode detection project is organized in a clear and modular structure. Below is a suggested file structure for the project:

vehicle-and-detection/
data/                    # Dataset directory (e.g., YOLOv4 weights, coco.names)
yolov4.weights        # Pretrained weights for YOLOv4
yolov4.cfg            # YOLOv4 configuration file
coco.names            # List of classes used by YOLOv4 (e.g., vehicle types)

detection.py          # Main detection script
README.md                # Project documentation


Key Files:

detection.py: This is the main file that runs the vehicle detection using YOLOv4. It processes input images or video streams, performs object detection, and displays results.

Library to download:

opencv-python (OpenCV for computer vision tasks)
numpy (Used for array manipulation)
psutil (For memory usage tracking)
matplotlib (For plotting results, optional)

Installation and Usage:

- Clone the repository
- Set up the virtual environment and dowload the libabry or just download
- Download the YOLOv4 weights
- Run detection.py

References and Documentation:

-YOLOv4 Paper
-YOLO Website

Issues and Contributions:


For the detection of trains and buses, especially trains, there are some difficulties sometimes. A more trained model on these two cases would be more optimal

Future Work:
The project has several potential avenues for improvement:

Improving Accuracy: Fine-tuning the YOLOv4 model with a custom dataset or using more advanced techniques like YOLOv5 or YOLOv7 could further improve accuracy.
Real-Time Optimization: The detection speed can be improved by using GPU acceleration (e.g., TensorRT or OpenVINO) or using a more lightweight model like YOLOv4-tiny for faster inference on edge devices.
Extended Dataset: The model can be trained on additional transport modes (e.g., trucks, bicycles, scooters) or different environments (e.g., night-time, weather conditions).
These improvements would make the system more robust and adaptable to a wider range of applications.