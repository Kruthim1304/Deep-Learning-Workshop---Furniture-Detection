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

<br>

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
-  

## Project architecture:
 <br>
<p align="center">
<img src = "" align="centre">
</p>	
<br>
	
	
## Mean average precision:
 <br>
<p align="center">
<img src = "![confusion_matrix](https://user-images.githubusercontent.com/83969166/171608625-cccb9b0a-5d1b-4a61-9889-924ab2f7329d.png)
" align="middle"><br>
</p><br>
As of a typical Conv2D model, we see that the accuracy keeps improving in performance compared to the baseline.


## Preview
<p align="center">
<img src="" width="800" height="400" />
<br>
<br>
</p><br>


<br>
# Contributors
	<br><br>


<a href="https://github.com/Kruthim1304/Deep-Learning-Workshop---Furniture-Detection/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=Kruthim1304/Deep-Learning-Workshop---Furniture-Detection" />
</a>

  
## License
[![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](http://badges.mit-license.org)

<p align=enter">
	Made with :heart: by <a href=""></a>
</p>
