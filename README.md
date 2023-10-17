# Car-Detection-by-YOLO
In this project, I implemented the YOLOv2 algorithm for car detection with a threshold of 0.72 using the Darknet19 model in Keras.
![Car_detect](https://github.com/HayLahav/Car-Detection-by-YOLO/assets/111200362/5e3fdf42-0045-4f45-96ca-6318b862cb92)

YOLO is an object detection algorithm that can detect multiple objects in an image and provide bounding box coordinates and class probabilities for each detected object.

Here's a brief breakdown of the main components and purposes of the code:

## 1) Model Architecture Definition:
* The code defines the architecture of the YOLOv2 model in Keras.
* It includes functions to create the Darknet-19 model and the YOLO head.

## 2) Loss Function:
* Defines the YOLO loss function used during training to optimize the model's parameters.
* The loss function includes terms for confidence loss, classification loss, and coordinate loss.

## 3) Model Evaluation:
* Provides functions for filtering and evaluating YOLO predictions based on confidence scores and non-maximum suppression.
* These functions are used to post-process the model's output during inference.

## 4) Utility Functions:

* Several utility functions for reading class names and anchors, generating colors, and drawing bounding boxes on images.
* The predict function takes an image, preprocesses it, runs it through the YOLO model, evaluates the output, draws bounding boxes, and saves the annotated image.

## 5) Pre-trained Model Loading:
* Attempts to load a pre-trained YOLOv2 model.

## 6) Model Prediction Loop:

Iterates over images in the "images" directory, predicts bounding boxes using the YOLO model, and saves annotated images to the "out" directory.
