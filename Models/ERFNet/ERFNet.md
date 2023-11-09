# ERFNet Architecture
## Overview
ERFNet stands for Efficient Residual Factorized Convnet. It makes use of three different modules that it stacks together.
1. A factorized residual network module with dilations.
2. A downsampling module inspired by an inception module.
3. An upsampling module.

![ERFNet Complete](https://github.com/Anoushka1009/Semantic_Segmentation/blob/main/Assets/Images/ERFNet%20complete.png)

Layer composition of the architecture: 

![ERFNet layers](https://github.com/Anoushka1009/Semantic_Segmentation/blob/main/Assets/Images/ERFNet%20layers.jpg)

## Blocks
### Encoder
The layers from 1 to 16 in our architecture form the encoder, composed of residual blocks and downsampling blocks.
Three downsamplings are performed at layers 1, 2 and 8.

**Residual networks** allow for very deep models to be created without as much risk of vanishing/exploding gradients. ERFNet makes use of Resnet modules but modifies them with the addition of two other deep learning techniques. It makes use of asymmetric factorized convolutions to make it more computationally efficient. It also makes use of dilated convolutions to give the layers in the network a lot of context.

**Factorization** can be used to break a higher dimensional convolution into a sequence of effectively lower dimensional convolutions which has a lower computational complexity and approximately the same result.

**Downsampling:** ERFNet downsampling module splits the input into two branches. On one branch, a 3×3 convolutional operation with a stride of 2 is applied, and along the other branch, a max-pooling operation is applied. The resulting outputs then get concatenated together to form the output of the module.

![Downsampling](https://github.com/Anoushka1009/Semantic_Segmentation/blob/main/Assets/Images/Downsampling%20block.png)

![Non-bottleneck 1D](https://github.com/Anoushka1009/Semantic_Segmentation/blob/main/Assets/Images/Non-Bottleneck%201D.png)

### Decoder
The decoder segment is composed of the layers from 17 to 23.
ERFNet follows a similar strategy to ENet in having a small decoder.
Deconvolution layers with stride 2 are used.

**Upsampling:** This module simply makes use of Transpose convolutions to regain the original image dimensions. 