# Our Project
Real-time implementation of Semantic Segmentation for traffic detection and autonomous driving applications. 
# Table of contents
- [About the Project](#About-the-Project)
  - [Tech Stack](#Tech-Stack)
  - [File Structure](#File-Structure)
- [Getting Started](#Getting-Started)
  - [Prerequisites and installlation](#Prerequisites-and-installlation)
  - [Installation](#Installation)
  - [Execution](#Execution)
- [Theory and Approach](#Theory-and-Approach)
-  [Results and Demo](#Results-and-Demo)
-  [Future Work](#Future-Work)
-  [Contributors](#Contributors)
-  [Acknowledgements and Resources](#Acknowledgements-and-Resources)

# About the Project
Aim of semantic segmentation is to accurately classify each pixel in an image into specific object or class categories, facilitating detailed scene understanding for various computer vision applications.

![Semantic Segmentation.png](https://github.com/Anoushka1009/Semantic_Segmentation/blob/main/Assets/Images/Semantic%20Segmentation.jpg)

> (Add here about the finalized realtime model)
## Tech Stack
- [Python](https://www.python.org/)
- [Opencv](https://opencv.org/)
- [Numpy](https://numpy.org/doc/#)
- [Tensorflow](https://www.tensorflow.org/)
- [Pytorch](https://pytorch.org/)
> (from tf and pytorch choose whichever is finalized for the model)
## File Structure
# Getting Started
## Prerequisites and installation
- Download Python on your device if not already present. 
 Refer [here](https://www.python.org/downloads/) for the setup.
- You can use any code editor.
- All installations mentioned are made using pip hence install pip.
  - To install pip , follow this [link](https://www.geeksforgeeks.org/how-to-install-pip-on-windows/)
- To install numpy
```
pip install numpy
```
- To install OpenCV
```
 pip install opencv-python
```
- To install Tensorflow
```
pip install tensorflow
```
- To install Pytorch
```
pip install pytorch
```
## Installation
- Clone the repository
```
git clone https://github.com/extint/Semantic_Segmentation.git
```

## Execution
After cloning the repository, you're all set to run it !
- Open your terminal and go to the same folder/directory where you cloned the repository
- Run
```
python3 <file_name>.py
```
# Theory and Approach
* We aim to use the **Convolutional Neural Network** approch over the traditional algorithms because CNNs can learn features automatically, work end-to-end, maintain spatial information, offer adaptability and transfer learning, and achieve state-of-the-art performance and hence are more effective and versatile for this task.
To know more about CNNs, go through [this document](https://github.com/Anoushka1009/Semantic_Segmentation/blob/d4b1e09b3fe3fc698ec354e0eeb075ec13a15f17/Implementation/Approach.md)

* Overview of the architecture used: 
The architecture we've chosen for real-time semantic segmentation is **MobileNetV2** because its efficiency is achieved through a combination of architectural innovations and design choices that reduce the model's computational complexity and memory footprint without sacrificing too much in terms of performance. It's an excellent choice for tasks like image classification, object detection, and more on mobile and embedded devices.
To learn more about the architecture used, click  [here](https://github.com/Anoushka1009/Semantic_Segmentation/blob/d4b1e09b3fe3fc698ec354e0eeb075ec13a15f17/Implementation/Architecture.md)

# Results and Demo

# Future Work

# Contributors
[Vedant Mehra]()
[Abhi Mehta]() 
[Anoushka Ruikar]()

# Acknowledgements and Resources
### Acknowledgements
We would sincerely like to express our heartfelt grattitude towards our mentors Smit Shah and Yatharth Dedhia for their valuable guidance throughout the project.
### Resources
 - [A Comprehensive Guide to Convolutional Neural Networks](https://www.v7labs.com/blog/convolutional-neural-networks-guide)
 - [MobileNetV2: Inverted Residuals and Linear Bottlenecks](https://arxiv.org/abs/1801.04381)
 

