# football_field_line_detection

This repository uses various techniques to detect field lines on an american football field. Furthermore it attempts to map a camera frame of the field to a bird's eye view map. Two approaches were used to detect lines: classical computer vision and neural network.

## Classical Computer Vision

The classical approach consists methods like the Hough Lines algorithm combined with linear algebra fundementals to detect and outline field lines. This is inspired of the work of [Junru Wang and Yuxuan Liu](https://mulab.ai/project/499-22-sports-analytics/).

## Neural Network

The [YOLOv8x](https://docs.ultralytics.com/) from Ultralytics was used as a foundation model. It was then fine-tuned on a football field feature dataset from [lucky-mesu2](https://universe.roboflow.com/lucky-mesu2/signs-dm6pe/dataset/3#) on Roboflow. Then various linear algebra techniques were used to determine lines and positions.
