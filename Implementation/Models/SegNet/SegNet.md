 # SegNet
![](/Assets/Images/segnet.png)
### Overview
SegNet is a convolutional neural network (CNN) architecture designed specifically for semantic segmentation tasks in computer vision. Its architecture is characterized by an encoder-decoder structure. In the encoder part, several convolutional layers are followed by max-pooling layers, which downsample the input image, extracting high-level features while reducing spatial dimensions. One of the distinctive features of SegNet is its use of max-pooling indices from the encoder in the decoder. These indices indicate the positions of the maximum values during pooling and are employed to guide the upsampling process in the decoder. This approach enhances the precise localization of object boundaries and details in the output segmentation map, which is crucial in semantic segmentation tasks. The architecture often includes a softmax layer at the end of the decoder to produce a probability distribution over different classes for each pixel in the segmentation map.
### Output
![](/Assets/Images/SegNet_out.png)
