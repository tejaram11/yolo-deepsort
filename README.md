# yolo-deepsort

To address the challenge of high-precision object tracking, we integrated YOLOv4's deep detection capabilities with DeepSort's real-time tracking within a TensorFlow environment. This results in a robust tracking solution.
We can take the output of YOLOv4 feed these object detections into Deep SORT (Simple Online and Realtime Tracking with a Deep Association Metric) in order to create a highly accurate object tracker.

# This project is based on The AIGuyscode yolov4-deepsort project.
Counting no of oranges in a video using DeepSORT algorithm 

Object Tracking implemented with DeepSORT, YOLOv4 and TensorFlow. A video containing the Instances of the fruits are carried on Detection.

1.Object Detection with YOLOV4:
    For purpose of Detecting the instances of Oranges, I have used YOLOv4 (You Look Only Once) model along with pretrained weights on coco dataset. This pre-trained YOLOv4 model can detect around 80 classes like person, car, apple, traffic signs etc. So for the given problem I have selected only class ‘orange’ in the dataset. This YoloV4 model can take 480*480 input size and returns bounding box for detected instances of the class orange.
    
2.Object Tracking with DeepSORT:
    After the bounding box is returned from yolov4 model, the detection results are then passed to DeepSORT tracker. DeepSORT uses COSINE distance to identify the instance throughout the frames. DeepSORT uses the bounding box along with a tracking ID for the instances. This tracking ID is used for counting the no. of oranges.

Refer to the document "DeepSORT_oranges.docx" for metrics and commands


