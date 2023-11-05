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
-  [Flowchart](#Flowchart)
-  [Results and Demo](#Results-and-Demo)
-  [Future Work](#Future-Work)
-  [Mini Projects](#Mini-projects)
-  [Contributors](#Contributors)
-  [Acknowledgements and Resources](#Acknowledgements-and-Resources)

# About the Project
Aim of semantic segmentation is to accurately classify each pixel in an image into specific object or class categories, facilitating detailed scene understanding for various computer vision applications.

![Semantic Segmentation.png](https://hackmd.io/_uploads/S1C69rB76.png)

> (Add here about the finalized realtime model)
## Tech Stack
- [Python](https://www.python.org/)
- [Opencv](https://opencv.org/)
- [Numpy](https://numpy.org/doc/#)
- [Tensorflow](https://www.tensorflow.org/)
- [Pytorch](https://pytorch.org/)
> (from tf and pytorch choose whichever is finalized for the model)
## File Structure
```
.📦
├── 📂assets				    # Contains images and videos		
│   ├── 📜images
|   ├── 📜result.mp4
├── 📂Clustering                            # contains code of kmeans and improved kmeans and its breif summary
|   ├── 📜Improved.py
|   ├── 📜K_Means.py 
|   ├── 📜README.md
├── 📂Initialization                        # codes and summary of initialization techniques
|   ├── 📜KMeans_Plus.py
|   ├── 📜README.md
|   ├── 📜Random.py
|   ├── 📜Subtractive_Clustering.py
├── 📜main.py                               # module to run code of your choice
├── 📂Processing                            # code to improve contrast
|   ├── 📜pcs.py
|   ├── 📜README.md 
├── 📂Results                               # Project result
|   ├── 📜Set1
|   ├── 📜Set2
|   ├── 📜Set3
|   ├── 📜Set4
|   ├── 📜Set5
|   ├── 📜Set6
├──  📂report				   # Project report
|   └── 📜report.pdf		
└──📜README.md		                   # Project readme
```
> Modify this file structure
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
To know more about CNNs, go through [this document](/-ZK0ztCFTj-bp6tUaRyjsQ)

* Overview of the architecture used: 
(write in brief about the architecture)
To learn more about the architecture used, click  [here](/1DEUUFKnSSeItjEf64O58Q)