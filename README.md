AI-Based Smart Campus Detection System

Available vs Occupied Seat Detection

This project is developed as part of the SWS405 – Applied Artificial Intelligence course. It focuses on building a Computer Vision Object Detection system to identify whether seats in a campus environment are available or occupied using deep learning techniques. The system uses a custom dataset collected from real campus locations, where images were manually annotated with bounding boxes to classify seats into two categories: available and occupied. The model is trained using the YOLOv8 (You Only Look Once) object detection algorithm, which is known for its balance between speed and accuracy, making it suitable for real-time applications.

Project Objective

The goal of this project is to develop an intelligent system that can: Detect seats in images using object detection Classify each seat as available or occupied Provide bounding boxes with confidence scores Support real-time smart campus applications This system can be applied in environments such as libraries, classrooms, and study areas to help students quickly find available seating.

Technologies Used

Python YOLOv8 (Ultralytics) OpenCV Roboflow (for dataset annotation and preprocessing) Google Colab (for training and experimentation)

Dataset

A custom dataset was created for this project, consisting of images captured in various campus environments under different lighting conditions and angles. Each image was annotated with bounding boxes and labeled into two classes:

Available Seat
Occupied Seat
The dataset ensures diversity and adheres to ethical guidelines by avoiding identifiable faces and personal data.

Key Features

End-to-end AI pipeline (data collection → annotation → training → evaluation → inference) Real-time object detection capability Custom dataset tailored for campus environments Model evaluation using precision, recall, and mAP

Code Explanation

Conclusion -Summary: This project successfully developed and implemented a Computer Vision object detection system for identifying available and occupied seats in campus environments. The system addresses a practical, real-world problem faced by students daily: the time wasted searching for available study spaces in libraries, classrooms, and other campus facilities.

The project achieved all its core objectives. A custom dataset of 600 images was collected from real campus locations, featuring diverse lighting conditions and camera angles. The dataset was carefully annotated with bounding boxes for two classes: available seats (300 images) and occupied seats (300 images) , maintaining strict ethical guidelines with no identifiable faces or personal data.

The YOLOv8 object detection algorithm was selected as the core model due to its proven balance between detection speed and accuracy, making it particularly suitable for real-time smart campus applications. The model was trained using Google Colab, with the training process taking approximately 9 hours to complete 100 epochs. The trained model successfully detects seats, classifies them as available or occupied, and outputs bounding boxes with confidence scores.

Key Findings: Several important findings emerged from this project:
. First, YOLOv8 proved to be an excellent choice for this use case. Despite the computational demands (9 hours of training), the resulting model demonstrates strong detection capabilities that would support real-time inference in a production environment. The trade-off between training time and inference speed is justified for this application.

. Second, dataset quality directly impacts model performance. By collecting 600 diverse images with balanced class representation (300 available, 300 occupied), the model received adequate exposure to both states under various conditions. The inclusion of multiple lighting conditions and angles helped the model generalize beyond the specific training examples.

. Third, manual annotation using Roboflow, while time-consuming, ensured high-quality bounding boxes. Consistent annotation practices across all 600 images provided the model with reliable ground truth data, which is essential for effective learning.

-Limitations: Despite the project's success, several limitations were identified:

. Training duration 9 hours of training time limits rapid iteration and hyperparameter tuning. . Fixed camera angles The model assumes consistent camera perspectives across deployment. . Lighting dependency Extreme lighting conditions (very dark, very bright) may reduce accuracy. . Limited seat types The dataset represents specific campus seating; new furniture may require additional training.

This project successfully applied modern machine learning and computer vision techniques to solve a tangible campus problem. A complete end-to-end AI pipeline was built, from custom dataset collection and annotation (600 images, 300 per class) to model training using YOLOv8 (9 hours on Google Colab) and final evaluation with bounding box visualization and confidence scoring.
