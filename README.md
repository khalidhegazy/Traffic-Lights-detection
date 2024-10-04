YOLOv8 Traffic Light Detection Project

Overview:

This project uses the YOLOv8 object detection model to identify and classify traffic lights in both images and videos. The model is designed to detect four different states of traffic lights: Red Green Yellow Off

The primary goal is: to demonstrate how a YOLOv8 model can be applied to real-world scenarios such as traffic monitoring and management by detecting and classifying traffic lights in various conditions.

Dataset:

The dataset consists of labeled images of traffic lights in the above four states. The dataset is structured for training, validation, and testing purposes: The images were labeled and annotated to correspond with the model's detection classes. The dataset folder contains subdirectories for training and validation images, each paired with corresponding annotation files.

Installation:

To run this project, the following libraries and dependencies are required: ultralytics (for YOLOv8) tensorflow (for model handling and exporting) opencv-python (for processing images and videos) gdown (to download the dataset) Once the dependencies are installed, the dataset can be downloaded and extracted.

Model Training:

The YOLOv8 model was trained for 60 epochs on a custom dataset with a resolution of 640x640 pixels. The training process involves feeding labeled traffic light images into the model, which then learns to classify and detect traffic lights.

The model was exported in a saved_model format after training, allowing for easy deployment and further inference.

Inference (Image and Video):

The trained model was used for inference on both images and videos. For images, the model was able to detect traffic lights, draw bounding boxes around them, and classify the lights based on their color and state (red, green, yellow, or off).

For video inference, specific frames from a traffic video were processed. The model detected traffic lights in those frames and marked them with bounding boxes. Additionally, the processed video was saved with annotations for detected objects, providing a visual understanding of how the model performed over time.

Results:

The model successfully detected traffic lights in various states across both images and video. While the small dataset was a limitation, the YOLOv8 model performed adequately in identifying the traffic lights in the validation and test samples.

Key Outcomes: Accurate detection and classification of traffic lights in images and videos. Clear visualization of bounding boxes and confidence scores on detected objects. Real-time performance was demonstrated on a sample traffic video, where multiple frames were processed and annotated.

Future Work:

To improve the model’s performance and accuracy, several areas of enhancement have been identified: Dataset Expansion: Adding more labeled images with different traffic light scenarios (e.g., different lighting, weather conditions, and traffic environments) will help the model generalize better.

Model Fine-Tuning: Additional fine-tuning and optimization could improve the detection accuracy, particularly for challenging conditions. Real-time Application: Optimizing the model's performance for real-time inference on video streams or integrating it with live traffic footage systems for broader deployment.

Conclusion This project demonstrated the successful implementation of the YOLOv8 model for detecting and classifying traffic lights. With further improvements, the model could be an essential tool for traffic management systems, helping automate traffic light detection in real-time for use in autonomous driving, traffic analysis, or surveillance systems.
