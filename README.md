<H1 align="center">Furniture Detection</H1>
<p align="center">
<a href="">
	<img src="https://media4.giphy.com/media/dWBM1IszT6hWNYXcU9/giphy.gif?cid=ecf05e47mqln7ifh2yo8w3r73ddpefwr1lah7cdmmqenq901&rid=giphy.gif&ct=s" width=80%/>
</a>
	<h2 align="center">   </h2>
	<h4 align="center">   <h4>
</p>

	
Computer vision is a rapidly growing field in the technology and computer science world.
An object detection system consists of recognizing, classifying, and localizing, not only one piece of furniture in an image but every referenced piece of the furniture mentioned.
One of the most popular algorithms to date for real-time object detection is YOLO (You Only Look Once). The great thing about this Deep Neural Network is that it is very easy to retrain the network on your own custom dataset.
In this project, we have made a custom dataset consisting of 6 classes of furnitures. They are as follows :
- Chair
- Table
- Sofa
- Bed
- Light Stand
- Shoe Table

In each class, there are around 160 labelled images for training our model. 
In total we have 977 images.

## Data preprocessing steps:
- Annotated Furniture Images
	- Data Source: Google Images ( web scraped )
	- Obtained around 977 images across 6 categories
	- The Images were labelled using LabelImg, object bounding boxes

## Model Construction:
-  For this project we have used YOLOv5 Model Architecture.
-  YOLO an acronym for 'You only look once', is an object detection algorithm that divides images into a grid system. Each cell in the grid is responsible for detecting objects within itself.
-  YOLO is one of the most famous object detection algorithms due to its speed and accuracy.

## Functionalities
-  It can be used to detect usable furniture such as  
	-  Chair
	-  Table
	-  Sofa
	-  Shoe Stand
	-  Bed
	-  Light Stand

## Instructions to run:

- If you want to train a custom model, clone [this](https://github.com/ultralytics/yolov5) repo, and follow [this](https://github.com/ultralytics/yolov5/wiki/Train-Custom-Data) link. You'll end up with the weights file of your custom trained model.
- In order to check your custom model, `cd yolov5` and run the below command:
	```bash
	python detect.py --source 0  # webcam
        	                  img.jpg  # image
                	          vid.mp4  # video
                        	  path/  # directory
                         	  path/*.jpg  # glob
                          	  'https://youtu.be/Zgi9g1ksQHc'  # YouTube
                          	  'rtsp://example.com/media.mp4'  # RTSP, RTMP, HTTP stream
	```
- Install Deepstream on the Jetson board.
- Once the PyTorch model works fine, follow [this](https://github.com/marcoslucianops/DeepStream-Yolo#yolov5-usage) link to convert the PyTorch model into cpp, and compatible with Jetson board, using Deepsteam.
- Run the below command to run the custom YOLOv5 model on Jetson, in real time:
	```bash
	deepstream-app -c deepstream_app_config.txt
	```

## Project architecture:

![project architecture](https://user-images.githubusercontent.com/83969166/171612620-0d884fb0-062a-4dbb-918d-479518f4d30a.jpeg)

</p>	
<br>
	
## Confusion Matrix:
![confusion_matrix](https://user-images.githubusercontent.com/83969166/171611558-fdb9344d-1c37-42c4-9518-4a2a0034c9b3.png)

## Training Metrics History

<p align="middle">
<img src="https://user-images.githubusercontent.com/34481342/172166264-b9481d63-f0b0-44f1-b387-82f9372fd62c.png" width=300>
<img src="https://user-images.githubusercontent.com/34481342/172166324-3903371a-4654-40fd-913e-f715b252093b.png" width=300>
<img src="https://user-images.githubusercontent.com/34481342/172166441-48b7d657-91b0-4172-a8dd-d0e933e32ee2.png" width=300>
<img src="https://user-images.githubusercontent.com/34481342/172166384-01dd3651-f769-48fa-92b6-b86924ef7565.png" width=300>
<img src="https://user-images.githubusercontent.com/34481342/172166507-e953952b-1dff-4420-851f-563fa5e6477a.png" width=300>
<img src="https://user-images.githubusercontent.com/34481342/172166579-f5a2b5bb-3c57-4e89-ba32-09383155ce05.png" width=300>
</p>

From the above graphs, we can see that the Mean Average Precision keeps increasing as we train the model for longer. The loss also goes down significantly.

## Preview

We have also attached a video of our model. Follow the link given below: 

https://drive.google.com/file/d/13aBa3yXtUdYtLMK0YUIBTHaB_fk9L4-J/view?usp=sharing

![1](https://user-images.githubusercontent.com/90834830/171609499-a40cbd61-836b-4005-8239-e7a53ccc0fc9.jpg)
<p align="center">

<br>
</p><br>

<br>

## License
[![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](http://badges.mit-license.org)

<p align="center">
	Made with :heart: by Groot_AI<a href=""></a>
</p>
