# Architecture 
## MobileNetV2
MobileNetV2 is a convolutional neural network architecture that seeks to perform well on mobile devices. It is based on an inverted residual structure where the residual connections are between the bottleneck layers. The intermediate expansion layer uses lightweight depthwise convolutions to filter features as a source of non-linearity. As a whole, the architecture of MobileNetV2 contains the initial fully convolution layer with 32 filters, followed by 19 residual bottleneck layers. 

![MobileNetV2](/Assets/Images/mobilenetv2.png)

Why is MobileNetV2 efficient?

1. **Depthwise Separable Convolutions:** MobileNetV2 uses depthwise separable convolutions, which are a more efficient alternative to traditional convolutions. In a depthwise separable convolution, the input is first convolved with a depthwise convolution (separate convolution for each channel), followed by a pointwise convolution (1x1 convolution) to combine the channels. This reduces the number of parameters and computations, making the model lighter and faster.

2. **Inverted Residuals:** MobileNetV2 introduces the concept of inverted residuals, which helps to capture more complex features with fewer parameters. Inverted residuals involve expanding the number of channels in the depthwise convolution, applying a non-linear activation function (e.g., ReLU6), and then reducing the number of channels with a 1x1 convolution. This expansion and reduction step helps the model capture more information without significantly increasing the computational cost.

3. **Linear Bottlenecks:** MobileNetV2 uses linear bottlenecks, where the channels in the network are increased linearly (i.e., the number of channels is doubled or tripled) instead of exponentially. This approach allows for a more balanced trade-off between model capacity and computational cost.

4. **Efficient Network Design:** MobileNetV2 employs an efficient architecture design, which includes factors like choosing optimal filter sizes, the number of layers, and the overall network depth. The network architecture is carefully crafted to achieve a good balance between accuracy and computational efficiency.

5. **Regularization Techniques:** MobileNetV2 incorporates regularization techniques like batch normalization and dropout to improve training and generalization performance while keeping the model efficient.

6. **Mobile-Friendly Parameters:** MobileNetV2 is designed to be lightweight and suitable for mobile devices. It aims to minimize the number of parameters and computational operations while maintaining good accuracy. This makes it well-suited for real-time applications on resource-constrained devices.
