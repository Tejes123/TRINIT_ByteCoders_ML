# TRINIT_ByteCoders_ML
## Automated Road Damage Detection for Infrastructure Maintenance
This repository contains the code and description of the solution of the problem statement in ML stream (ML_01) : Automated Road Damage Detection for Infrastructure Maintenance
## Problem Statement Description
Manual inspection of road conditions is a time-consuming and labor-intensive
task, leading to delays in identifying and repairing damaged roads. The goal is to
develop a classification model capable of automatically detecting and
categorizing road damage from images (captured through CC
cameras,phone,etc.), in order to make the maintenance process efficient. The
infrastructure management is enhanced by reducing the reliance on manual
inspections and enabling timely and targeted repairs to ensure safe and
well-maintained road networks
## Objective
The dataset has images of roads with background. The model should
involve object detection to capture only roads (using YOLO or R-CNN or
their combination,etc.), followed by classifying the damaged roads
![Image](/example.png)
## Dataset
We have trained a model in the RDD2022_India dataset provided. The model was not trained well on the datset and the annotations are not good. WE even used RDD2022_Japan to train another model, but we faced more computational power requirement. So we chose to use some custom datasets available
### Dataset Description
We have used a dataset that contains the 2.5K images of roads with potholes with annotations. We trained a YOLO5 model in google colab on the dataset mentioned here, as our PC/s dont meet the computational requirements. The dataset used in the project can be found here: [https://universe.roboflow.com/potholes-detection-zdxgw/pothole-jujbl](https://universe.roboflow.com/potholes-detection-zdxgw/pothole-jujbl)
## Model
We used a YOLO5 model to detect the potholes in the images. We used the repository whose link is given below to build the model.[] After training we get weight file named best.pt 
## Video Demo
The video demo of how our project works can be seen here [Video Link](https://drive.google.com/file/d/12UcH7yAfSLC51zBQ0DXfktxFyVDF2iT_/view)
## Evaluation metrics
model MAE(mean Average precission) is over 90%
## How to run the model
Only run detect.py to run the model.
## Reference
1. [https://colab.research.google.com/drive/1vBKloRTjCoVwNIZLmxZxh_DPn-ja0_gG?usp=sharing](https://colab.research.google.com/drive/1vBKloRTjCoVwNIZLmxZxh_DPn-ja0_gG?usp=sharing)
2. [https://github.com/ultralytics/yolov5](https://github.com/ultralytics/yolov5)
3. Other sources in internet


