#Convolutional Neural Network (CNN)
The common Set-up of the CNN :
in order to implement CNNs, most successful architecture uses one or more stacks of convolution + pool layers with relu activation, followed by aflatten layer then one or two dense layers.

<img src="https://cv-tricks.com/wp-content/uploads/2017/05/vgg16.png"  />

<br/>
Convolutional Neural Network (CNN) is a class of deep neural network (DNN) wich is widely used for computer vision or NLP. During the training process, the network's building blocks are repeatedly altered in order for the network to reach optimal performance and to classify images and objects as accurately as possible. 
Convolutional neural networks excel at learning the spacial structure in input data.
<br/>
## CNN layers <br/>
### Convolutional layer: 
Finding the features and apply filters 
<img src="https://miro.medium.com/max/526/1*ZCjPUFrB6eHPRi4eyP6aaA.gif"  />
Parameters that control the behavior of each convolved layer
*Stride
*Padding (Zero-padding)
*Number of filter (depth of next layer)
*Size of the filter
### Activating function : ReLU
ReLu less computationally expensive than Tanh and Sigmoid: ReLU improve neural networks by speeding up training. The gradient computation is very simple (either 0 or 1 depending on the sign of x). Also, the computational step of a ReLU is easy: any negative elements are set to 0.0 -- no exponentials, no multiplication or division operations
### Max Pooling :
Downsize the image and keep the important features. 
Spacial Pooling (also calld subsampling or downsampling) reduces the dimensionality of each feature map and retains the most important information of an image. Spatial Pooling can be of different types : Max, Average, Sum, etc.
<br\>
### Faltting :Convert to 1 dimension array (vector)
Therefore you need to convert the output of the convolutional part of the CNN into a 1D feature vector, to be used by the ANN part of it.
### Full Connection 
Building all needed connections

Convolution in 3D:
Applied in the Same way as 2D (sum of weight*pixel value as they slide across the image )