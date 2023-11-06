# CNNs
A CNN is a kind of network architecture for deep learning algorithms and is specifically used for image recognition and tasks that involve the processing of pixel data.

**CNN network components:**
The general architecture of a CNN involves alternating convolutional and pooling layers to extract hierarchical features from the input data which are then flattened and passed through one or more fully connected layers to make final predictions. 

![CNN](https://github.com/Anoushka1009/Semantic_Segmentation/blob/dc1c1aab1235520f1d2d99e07a1b570c7bce9396/Assets/Images/CNN.png)


1. **Input Layer:** The input layer accepts the raw data, a grid of pixel values that represent corresponding pixel’s intensity or colour information.

2. **Convolutional Layers:** Apply convolutional operations to the input data to extract features. A convolution involves sliding a small filter/kernel over the input data and summing the results of element-wise multiplication. This helps identify patterns, edges, textures, and other features in the data. 

3. **Activation Function:** After the convolution, an activation function like ReLU (Rectified Linear Unit) is often applied element-wise to the output of the convolutional layer to introduce non-linearity. This helps the network learn more complex patterns. There are other activation functions as well like Sigmoid, Leaky ReLU, Softmax, etc. 

4. **Pooling Layers:** Pooling layers downsample the feature maps, reducing their spatial dimensions while retaining important information. Common pooling techniques include max pooling and average pooling.

5. **Fully Connected Layers:** Fully connected layers (dense layers)are used to make final predictions or classifications based on the extracted features. These layers connect every neuron in one layer to every neuron in the next layer.

6. **Softmax activation:** Activation functions like softmax are applied to generate probabilities for each class.

7. **Output Layer:** The output layer produces the final predictions of the network. The number of neurons in this layer denotes the number of classes or categories in the classification task.

# Architecture 
## MobileNetV2
MobileNetV2 is a convolutional neural network architecture that seeks to perform well on mobile devices. It is based on an inverted residual structure where the residual connections are between the bottleneck layers. The intermediate expansion layer uses lightweight depthwise convolutions to filter features as a source of non-linearity. As a whole, the architecture of MobileNetV2 contains the initial fully convolution layer with 32 filters, followed by 19 residual bottleneck layers. 

![MobileNetV2]()
