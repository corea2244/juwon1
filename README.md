# DLIP LAB4

# 1. Subject
### Automatic key limitation measurement program when boarding rides in amusement parks.




# 2. Background
#### There are many rides in the amusement park with height restrictions. Failure to comply with height restrictions can lead to safety accidents immediately. There are many people who want to board without complying with the height limit, and it is difficult for amusement park staff to check all of them. If you can recognize a person through a camera and measure his or her height in real time while standing in line at an amusement park, it can help prevent safety accidents. In addition, if the height limit is violated, an alarm may be displayed to determine whether it is possible to board easily and quickly.


# 3. Theory
## > 1. yolov5
#### Conventional yolov3 had higher frame per seconds (FPS), while mean average precision (mAP) was a relatively lower model. However, yolov5 outperforms both in terms of FPS and mAP. And unlike other models of the yolo, the yolov5 is divided into sizes.  Yolov5s, Yolov5m, Yolov5l, Yolov5x, which is easy to distinguish if you think of it as small, medium, large, and xlarge.  This division is the difference between depth multiple (model multiple) and width multiple (layer width multiple).
<img src="./yolov5.png" width="450px" height="300px" title="Yolov5 Performance Comparison Table"></img><br/>
#### Accuracy and speed are conflicting and cannot be caught altogether. Instead of s being the fastest, accuracy is reduced and x being the slowest, accuracy is improved. The reason why YOLOv5 is faster than the existing YOLO series is the difference between backbone and head. The Backbone part extracts Feature Map from the image, similar to yolov4. The point here is that we used CSPNet. The head part is to locate an object based on Feature Map. The Anchor Box (Default Box) is initially set up and then used to create the final bounding box. We generate bounding boxes on three scales and use three anchor boxes on each scale.

2. Coco dataset
#### We present a new dataset with the goal of advancing the state-of-the-art in object recognition by placing the question of object recognition in the context of the broader question of scene understanding. This is achieved by gathering images of complex everyday scenes containing common objects in their natural context. Objects are labeled using per-instance segmentations to aid in precise object localization. Our dataset contains photos of 91 objects types that would be easily recognizable by a 4 year old. With a total of 2.5 million labeled instances in 328k images, the creation of our dataset drew upon extensive crowd worker involvement via novel user interfaces for category detection, instance spotting and instance segmentation. We present a detailed statistical analysis of the dataset in comparison to PASCAL, ImageNet, and SUN. Finally, we provide baseline performance analysis for bounding box and segmentation detection results using a Deformable Parts Model
-	Train2017 (19G)
-	Val2017 (788M)
-	Test2017(6.3G)
-	Annotations(808M)


# 4. Process

# 5. Code

# 6. Analysis

# 7. Limit

# 8. Conclustion
