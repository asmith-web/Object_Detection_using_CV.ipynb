Object Detection locates objects in an image and labels them with a class + confidence. It's broader than classification because detection retruns where each object is.

Why YOLOv8?
YOLOv8 is a modern, easy-to-use implementation of YOLO family with a simple Python API for inference & training. Excellent for teaching quick demos and moving to custom datasets.

Real-World Examples
* Autonomous vehicles: detect pedestrians, cars, traffic signals.
* Retail: shelf monitoring, automated checkout.
* Industrial inspection: detect defective parts on a conveyor.
* Security: detect intruders, suspicious objects in CCTV feeds.


This project uses the YOLOv8 object detection model from the ultralytics library to identify objects in an uploaded image. Here's a breakdown of the steps:

Setup: The first cell installs the necessary libraries: ultralytics for YOLOv8, opencv-python-headless for image handling, and matplotlib for displaying the results.
Image Upload: The second cell allows you to upload an image file. The path to the uploaded image is stored in the img_path variable.
Model Loading and Inference: The third cell loads a pre-trained YOLOv8-nano model (yolov8n.pt). It then runs the model on the uploaded image (img_path) to detect objects. The results are stored in the result variable.
Visualization: The final cell takes the first result from the inference (res0), moves the data to the CPU, and then uses the built-in plot() method to draw bounding boxes and labels around the detected objects. Finally, it displays the annotated image using matplotlib.
